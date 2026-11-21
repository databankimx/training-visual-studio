# The test project

Open the practice solution and look in the Solution Explorer. The solution has three projects: Pricing, PriceReport, and Pricing.Tests. Pricing.Tests is a test project. It does not ship with the program. Its only job is to call the code in Pricing and check the answers.

Open Pricing.Tests, then PriceCalculatorTests.cs. The file uses NUnit, a popular test framework for .NET. Three parts appear in every test:

- The attribute [TestFixture] above the class marks the class as a group of tests.
- The attribute [Test] above a method marks that method as one test.
- Assert.That compares the result with the answer you expect.

Each test has three steps. First it sets up the input, then it calls the method, then it asserts the answer. Here is the Average test, with the comment lines removed:

```csharp
[Test]
public void Average_OfTwoAndFour_IsThree()
{
    decimal result = PriceCalculator.Average(new[] { 2m, 4m });
    Assert.That(result, Is.EqualTo(3m));
}
```

The name says what the test checks. When a test fails, the name tells you what broke before you open the file. A name like Average_OfTwoAndFour_IsThree is far more useful than Test1.

Pricing.Tests references the Pricing project, so the test can call PriceCalculator directly. The test project does not need its own copy of the code.

## Try it

1. In Solution Explorer, expand Pricing.Tests, and open PriceCalculatorTests.cs.
2. Press {{Ctrl+T}}, type Average_OfTwoAndFour, and choose the method. Find the three steps in the body of the test.
3. Count the tests in the file. There are five. You will run them in the next lesson.
