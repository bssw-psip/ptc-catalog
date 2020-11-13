# THG Coding Standards

## Target

Steadily convert the codebase over to an agreed-upon stand.

## User Story

As a person responsible for software quality and correctness for the HDF5 library, I want guidance on selecting and implementing coding standards so that we can make our code easy for everyone to read and understand.

As an HDF5 library developer or community contributor, I want tel support so that I man complying with the standards with minimal additional effort or ambiguity.


## Card

| Score | Description |
|:-----:|:------------|
| 0 | No coding standard adopted. See *Tasks to Reach Score 1*, below. |
| 1 | The team has selected and documented an agreed-upon standard.  |
| 2 | New code that is written is required to comply with the standard, and the team has conducted a feedback session to assess and revise the standard. |
| 3 | The team has developed and put into place a refactoring plan to bring preexisting code into compliance with the standard. |
| 4 | Tool support has been put in place to help ensure compliance, and running the tool is made part of the contribution process. |

### Tasks to Reach Score 1

- [ ] Select representative source files
- [ ] Create outlines for Best practices and HDF5 things
- [ ] Review different standards and use clang-format tool to reformat selected files.
- [ ] Present finding to HDF developers and select HDF5 C coding standard
- [ ] Review feedback and modify yml files used by format tool
- [ ] Document deviations from the standard and create HDF5 style sheet.
- [ ] Publish HDF5 C coding style
- [ ] Enable automatic checks (via Actions) on PRs and check-ins in GitHub
- [ ] Complete HDF5 things document
- [ ] Publish Best Practices document
- [ ] Publish HDF5 things document

## Related Cards

- [THG GitHub Migration](THGGitHubMigration.md)
- [THG Reference Manual](THGReferenceManual.md)

## Other Remarks

This card was created by the [THG PSIP Pilot project](https://www.osti.gov/biblio/1698291-psip-hdf5pilot-project-final-report).
