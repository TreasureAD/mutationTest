# Mutation Testing Report

## 1. Introduction
This report presents the findings from the mutation testing process conducted on the `Polynomial` class using MutPy. Mutation testing aims to evaluate the efficacy of the test suite by introducing controlled mutations to the source code and analyzing the test outcomes.

## 2. List of Defined Mutation Operators
The mutation operators defined for this analysis include:
- **Change Coefficients:** Modifying coefficients in the polynomial.
- **Arithmetic Operation Mutation:** Altering arithmetic operations.
- **Redundant Code Mutation:** Introducing redundant logic.
- **Boundary Mutation:** Modifying boundaries in root-finding methods.

## 3. Description of Applied Mutations and Their Impact
Mutations were applied to the `Polynomial` class utilizing MutPy. These alterations included changing coefficients by replacing values, modifying arithmetic operations within methods, introducing redundant loops, and altering boundaries in root-finding methods to test edge cases.

## 4. Summary of Mutant Survival and Killing
Upon running MutPy with the extended test suite, the mutation score increased to 56.5%. Out of 89 generated mutants:
- **Killed:** 26 mutants (29.2%)
- **Survived:** 20 mutants (22.5%)
- **Incompetent:** 43 mutants (48.3%)

## 5. Analysis of the Test Suite's Effectiveness
The updated test suite showed improvements in detecting mutations, leading to a higher mutation score. However, there is still a substantial number of incompetent mutants. This implies the need for further test coverage enhancement, especially around edge cases and arithmetic operations.

## 6. Recommendations for Improving the Test Suite
To boost mutation testing effectiveness and overall test coverage:
- Incorporate additional test cases targeting surviving mutants and boundary scenarios.
- Focus on testing arithmetic operations thoroughly, including corner cases.
- Implement more diverse and complex test cases to cover various mutation scenarios.
- Consider using property-based testing to validate multiple scenarios efficiently.

## 7. Conclusion
The mutation testing process using MutPy indicated a moderate improvement in mutation score after enhancing the test suite (test cases in PyTest.py). However, a considerable number of mutants remained undetected or exhibited incorrect test results. Enhancements to the test suite will be pivotal to further improve mutation score and overall code reliability.

Below are all of my added test suites to help improve the mutation score:



