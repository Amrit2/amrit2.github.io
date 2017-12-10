---
layout: post
title: 4 Rules of Simple Design
permalink: /simpledesign/
---
The 4 rules of simple design helps you to refactor in the TDD process so that your code is clean.

## Rules:
1. Test Pass -> The tests should pass and hence carry out the functionality it is required to before the other
rules are applied as there is no point in cleaning up if the tests are failing.

2. Small -> The code should be precise and should not have pieces of code that you don't need.

3. Expresses Intent -> Your code should should use names that describe what they do and therefore 
the code should be understandable instantly, hence express the intent well.

4. No Duplication (DRY) -> Don't Repeat Yourself. The code should not have any duplication of intent or duplication of knowledge.