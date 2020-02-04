# Promote User Confidence in Software Updates 

## Target

Ensure users are confident of application performance and behavior changes made by an update/new release.

## User Story

As a software engineer I want to instill user condfidence in updating the application
so that the latest application release is adopted. 

## Card

| Score         | Description |
| :-------------: | :------------- |
| 0 | There is minimal communication about application updates that does not always include behavior or performance changes. Users are not able to easily return to a prior version of the application after an update. |
| 1 | Application **behavior changes** are recorded to a single location. |
| 2 | Application **performance changes** are recorded to a single location or database. |
| 3 | As changes are made to the code base, recorded behaviors and performance changes are included in the release notes. |
| 4 | Document how users can obtain previous behavior. |
| 5 | Release notes are advertised to users, including behavior and performance changes, before each release. |

## Comments
- Item 2: Can be implemented using Github issues, Jira or other means to be able to follow what each release includes. 
- Item 3: See the [Performance Regression Testing card](https://github.com/bssw-psip/ptc-catalog/blob/master/catalog/PerformanceRegressionTesting.md)
- Item 4: Could be something like turning a new feature on or off, setting a configuration variable to have a previous behavior, or a link to a prior release.
