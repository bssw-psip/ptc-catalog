# Test Coverage



| Score         | Description |
| :-------------: | :------------- |
| 0 | Little or no independent testing. Functional testing via users. |
| 1 | Independent functional testing of primary capabilities.      |
| 2 | Primary functional testing, some unit test coverage.      |
| 3 | Comprehensive unit testing, primary functional testing.      |
| 4 | Comprehensive unit testing, functional testing for documented use cases.      |
| 5 | Comprehensive unit, use case functional testing; test coverage commitment.     |

## Comments

1. **Functional testing**: Testing capabilities from user's perspective.  Many functions can be called.  Good for usability assurance.  Insufficient to protect against some regressions.  Difficult to isolate regressions.  Can require extensive test execution times.
2. **Unit testing**: Isolated, independent testing of functions and methods.  Enable test-driven development, rapid test execution, fault isolation.  Insufficient to ensure functional correctness.
3. **Comprehensive**: Does not mean 100% line coverage, but sufficient coverage to detect most errors.  Experts suggest various metrics such as 80% or more line coverage, or some similar high percentage of function point coverage.
4. **Commitment**: Team is committed to writing comprehensive tests concurrent with functionality.
