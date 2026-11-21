# Writing a snippet

You can write your own snippet. A snippet file ends in .snippet and holds XML. The file has three parts to fill in: a header with a title and a shortcut word, a list of the placeholders, and the code.

Here is a small snippet that declares a decimal price. Save it as money.snippet in a folder you will find again, such as your Documents folder.

```xml
<?xml version="1.0" encoding="utf-8"?>
<CodeSnippets xmlns="http://schemas.microsoft.com/VisualStudio/2005/CodeSnippet">
  <CodeSnippet Format="1.0.0">
    <Header>
      <Title>Money</Title>
      <Shortcut>money</Shortcut>
      <Description>Declares a decimal price.</Description>
      <Author>Practice</Author>
    </Header>
    <Snippet>
      <Declarations>
        <Literal>
          <ID>price</ID>
          <ToolTip>The name of the price</ToolTip>
          <Default>price</Default>
        </Literal>
      </Declarations>
      <Code Language="CSharp"><![CDATA[decimal $price$ = 0m;]]></Code>
    </Snippet>
  </CodeSnippet>
</CodeSnippets>
```

The Shortcut is the word you type before you press {{Tab}} to insert the snippet. The Literal section declares a placeholder, and its ID must match the name between dollar signs in the code, so $price$ becomes whatever name you type. The code sits inside CDATA, which lets you write characters such as < and & without escaping them.

To use the file, open the Tools menu, and choose Code Snippets Manager. Set the Language to Visual C#, click Import, and choose money.snippet. Visual Studio copies the snippet into your snippets folder, and it appears in the picker.

Try the new snippet by typing money in a class, and pressing {{Tab}} twice.

## A real example to read

Many snippets are longer than money, and they show the same parts. This one inserts a try, catch, and finally block. It has no placeholders, so its Literal section is missing, and it has no shortcut, so you insert it from the picker.

```xml
<?xml version="1.0" encoding="utf-8"?>
<CodeSnippets xmlns="http://schemas.microsoft.com/VisualStudio/2005/CodeSnippet">
  <CodeSnippet Format="1.0.0">
    <Header>
      <SnippetTypes>
        <SnippetType>Expansion</SnippetType>
      </SnippetTypes>
      <Title>TryCatch</Title>
      <Author>Practice</Author>
      <Description>Insert a try/catch/finally block</Description>
      <HelpUrl>
      </HelpUrl>
      <Shortcut>
      </Shortcut>
    </Header>
    <Snippet>
      <Code Language="csharp" Delimiter="$"><![CDATA[
    <!-- The C# code from the block below goes here, between the CDATA markers -->
]]></Code>
    </Snippet>
  </CodeSnippet>
</CodeSnippets>
```

The code inside the CDATA markers is ordinary C#. It is shown here on its own, so you can read it with its colors:

```csharp
try
{
    // Your code goes here
}
catch (Exception ex)
{
    while (ex != null)
    {
        Console.WriteLine(ex);
        ex = ex.InnerException;
    }
}
finally
{
    // Final instructions here
}
```


Read it from the top. SnippetType of Expansion means the snippet is inserted at the cursor. The Title is the name the picker shows. The Shortcut is empty, so the snippet has no typed word and you choose it from the picker. The Code element holds the block itself, and the Delimiter of $ tells Visual Studio which character marks a placeholder. This block has none, so nothing needs filling in. Once inserted, the text is ordinary code, and you edit it like any other.

## Try it

1. Create money.snippet with the XML above, and save it.
2. Import it with the Code Snippets Manager.
3. Type money in a class, press {{Tab}} twice, and type a name for the placeholder.
4. Save the TryCatch snippet as TryCatch.snippet, with the C# from the second block between the CDATA markers, import it, and insert it from the snippet picker. Undo the insert with {{Ctrl+Z}}.
