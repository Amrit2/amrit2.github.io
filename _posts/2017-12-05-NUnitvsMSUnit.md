---
layout: post
title: NUnit vs MSUnit Testing
permalink: /testingmethods/
---
## MSUnit Testing

 The tags [TestClass] and [TestMethod] allows the VS to recognise that it's a test method.

`[TestClass]
public class Calculator
{
  [TestMethod]
  public class AddThreeAndFive()
  {
   Calc = new Calculator();
   result = Calc.Add(3,5);
   Assert.AreEqual(8, result);
  }
  [TestMethod]
  public class AddFourAndSix()
  {
   Calc = new Calculator();
   result = Calc.Add(4,6);
   Assert.AreEqual(10, result);
  }
}`

## NUnit Testing

The tags [TestFixture] and [TestCase] allows the VS to recognise that it's a test method.

`[TestFixture}
public class Calculator
{
  [TestCase (3,5)]
  [TestCase (4,6)]
  public class Add(int firstNumber, int secondNumber)
  {
   Calc = new Calculator();
   result = Calc.Add(firstNumber,secondNumber);
   Assert.AreEqual(8, result);
  }
}`


MSUnit requires you to rewrite the test to test different input whereas with NUnit you don't repeat yourself as the different inputs can be passed into the same test as parameters.
This eliminates repetition in your code.