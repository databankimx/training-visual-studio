# The Object Browser

Go to Definition works for code in your solution. The Object Browser works for everything else, such as the types in the .NET libraries that your code uses. It lists the namespaces, the types inside them, and the members of each type, so you can see what a library offers before you call it.

## Opening the Object Browser

Choose View, then Object Browser, or open Command Search with {{Ctrl+Q}} and type Object Browser. The window opens with a tree on the left, listing the assemblies your solution uses. Expand an assembly to see its namespaces, and expand a namespace to see its types.

## Try it

1. Open the Object Browser.
2. In the search box, type Decimal, and press Enter.
3. Open the result for the Decimal type. Read its members on the right, such as the methods that round a number.
4. Find the Pricing assembly in the tree, and expand it to see PriceCalculator, which is code from this solution.

## Using the Object Browser with your own code

The Object Browser also lists your own types, once the solution has built. Use it to check that a method has the name and parameters you expect, especially when a call in another project does not compile.

## Common mistake

The Object Browser shows what a type offers, but it does not show how a member is used. For a worked example, read the documentation for the type, or use Find All References in your own solution to see how your code calls it.
