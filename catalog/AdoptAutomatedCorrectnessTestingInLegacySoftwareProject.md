# Adopt Automated Correctness Testing in a Legacy Software Project

## Target

Adoption of automated testing for a [legacy software project](https://bssw.io/items/working-effectively-with-legacy-code) that has no automated tests at the beginning (e.g., where testing is done manually or only tested against customer codes).

## User Story

As a developer on a legacy software project/product, I want my team to adopt increasingly more rigorous and effective automated correctness testing, so that development will be easier, users will see less defects, releases will go out faster, and the sustainability of my project will be improved.

## Card

| Score | Description | Added Value |
| :---- | :---------- | :---------- |
| *0* | One or more automated simple [system-level tests](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingWhatIsDefinitionandCategorizationofTestsforCSESoftware-V0.2.pdf) that simply run the code for a few different inputs and look for 0 return code (i.e., does not crash) are created | Major breakages in the code causing segfaults and other crashes will be caught when code is changed or added. |
| *1* | Comparison of the code outputs to previous outputs are used to create [system-level no-change tests](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingWhatIsDefinitionandCategorizationofTestsforCSESoftware-V0.2.pdf). | Changes in the behavior of the code will be caught when code is changed or added. (But such tests can be very fragile.) |
| *2* | [System-level verification tests](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingWhatIsDefinitionandCategorizationofTestsforCSESoftware-V0.2.pdf) that don't just compare to previous output but instead look for physical or mathematical properties of the underlying equations or algorithms are added. | Good changes (like solving the equations to a higher tolerance faster) will not cause the tests to fail and these tests will be more robust compared to no-change tests. |
*3* | Developers use the [Legacy Software Change Algorithm](https://bssw.io/items/working-effectively-with-legacy-code) to make changes to existing code which tests larger integrated components creating [integration-level no-change/characterization tests](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingWhatIsDefinitionandCategorizationofTestsforCSESoftware-V0.2.pdf). | Changes to the code can be made faster and with less risk compared to only running system-level tests. |
| *4* | Developers use the [Legacy Software Change Algorithm](https://bssw.io/items/working-effectively-with-legacy-code) to make changes to existing code for for smaller units creating [unit-level non-change/characterization tests](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingWhatIsDefinitionandCategorizationofTestsforCSESoftware-V0.2.pdf) in addition to integration-level tests where appropriate. | Changes to the code can be made faster and problems will be easier to debug when compared to only writing tests at the courser-grained integration level. |
| *5* | Developers add automated [unit-level and integration-level verification tests](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingWhatIsDefinitionandCategorizationofTestsforCSESoftware-V0.2.pdf) for new code as it is written (or before it is written using Test Driven Development). | New code will have automated finer-grained tests which will make it easier and safer to extend that code in the future (and new code will no longer be "Legacy Code"). |

## Comments

* The testing definitions are given in the document [Definition and Categorization of Tests for CSE Software](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingHowtoAddImproveTestinginyourCSESoftwareProject-V0.2.pdf)
* More details about adding testing to an existing legacy project are given in [How to Add and Improve Testing in Your CSE Software Project](http://ideas-productivity.org/wordpress/wp-content/uploads/2016/04/IDEAS-TestingHowtoAddImproveTestinginyourCSESoftwareProject-V0.2.pdf).
* The "Legacy Software Change Algorithm" is defined and explained in great detail in the book ["Working Effectively with Legacy Code"](https://bssw.io/items/working-effectively-with-legacy-code) by Robert Martin.

## Related Cards

* The PTC card [Continuous Integration](https://github.com/bssw-psip/ptc-catalog/blob/master/catalog/ContinuousIntegration.md) describes steps/levels in how to take an existing set of automated tests and how run them, how to display their results, and how to use them to gate different development, integration, and other processes.
* The PTC card [Test Coverage](https://github.com/bssw-psip/ptc-catalog/blob/master/catalog/TestCoverage.md) is similar to this PTC card except this PTC card is consistent with advice in the book ["Working Effectively with Legacy Code"](https://bssw.io/items/working-effectively-with-legacy-code) by Robert Martin in that it does not expect that detailed unit tests will be added to cover all of the existing legacy code and that is okay.
* The PTC card [Test Driven Development](https://github.com/bssw-psip/ptc-catalog/blob/master/catalog/TestDrivenDevelopment.md) describes the phased introduction on test driven development and would seem to mostly apply to new code that is being written but does not address changes to existing code.
