# Integrated Software Documentation

## Target

Ensure that the user/developer documentation is fully integrated with the associated software.

## User Story

As a user (developer of software in this case), I want it to be easy to update documentation as I 
update the software the documentation describes. Typically, this means I want the software and documentation to be 
in the same place (e.g. repository). By easily, I mean handling things like images, in-line code, equations and cross 
references are a) possible and b) the same processes to manage changes to the code also works for the documentation. 
I don't have to learn a wholly separate content management system to manage documentation.

## Card

| Score         | Description |
| :-------------: | :------------- |
| 0 | Documentation is housed in the same repository as the code. |
| 1 | The documentation is text-based, ascii files (as well as perhaps binary images), just as the code is. |
| 2 | There is developer documentation and user documentation and the two are sufficiently organized so as not to cause these different classes of consumers to confuse the two. |
| 3 | Changes to code that have impacts on users (or developers) DO NOT get committed without associated changes to documentation. |
| 4 | The documentation covers (think of code coverage for testing) a majority of the functions the software performs. Key usage scenarios are not left UNdocumented. Perhaps different functionalities are weighted as to importance for either user-level or developer-level documentation. |
| 5 | There are working examples of the software and those examples are documentated such that the examples are routinely tested along with the software to ensure they still work. |
| 6 | Where appropriate code cross-references documentation and documentation cross-references code. |
| 7 | Documentation is versioned and different versions of the documentation are available for different versions of the software. |
| 8 | Documentation is part of the packaged release of the code such that, on air-gapped networks for example, it is carried along with the code release so that users on those networks do not have to shop elsewhere to find/host the documentation. |

## Comments
Some useful technologies to consider are

* [Markdown](https://en.wikipedia.org/wiki/Markdown) (there are many variants)
* [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/) and [GitHub pages](https://pages.github.com) 
* [Sphinx](http://www.sphinx-doc.org/en/master/)
* [ReadTheDocs](https://readthedocs.org)
* [Jekyll](https://jekyllrb.com) and Jekyll's [Documentation Theme](https://jekyllthemes.io/jekyll-documentation-themes)
