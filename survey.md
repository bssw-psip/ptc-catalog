<head>
<script language="javascript">
window.onload=function(){
var inputs = document.getElementsByClassName('survey'),
    total  = document.getElementById('survey-total');

 for (var i=0; i < inputs.length; i++) {
    inputs[i].onchange = function() {
        var add = this.value * (this.checked ? 1 : -1);
        total.innerHTML = parseFloat(total.innerHTML) + add
        var new_total = parseFloat(document.getElementById('input').value);
      console.log(new_total);
        document.getElementById('input').value=new_total + add
    }
  }
}
</script>
</head>

# Rate Your Project Survey

Brought you by the [IDEAS-ECP project](https://ideas-productivity.org) and the [PSIP Development Team](https://bssw.io/psip).

## Why are Software Team Practices Important?

Software engineering is a systematic approach to the design, development, and maintenance of a software system. Building reliable and maintainable software is difficult and expensive. By adopting a systematic approach to software development, it is possible to maximize the cost effectiveness of the software system.

### Key Objectives of Software Engineering

Objective | Description
:--------:|:-----------
Maintainability | Should be able to evolve to meet changing requirements
Correctness | Correctly implements the user requirements
Adaptability | Can be changed to adapt to new system or user constraints
Reusability | Modules can be readily reused to develop new software products
Testability | Should be testable with minimal effort
Portability | Can be cost effectively transferred from one computer system to another
Reliability | Should be able to perform its desired function over an arbitrary time period

<div style='page-break-after:always'></div>

### How Does Your Team Score?

Use the following survey to rate your team practices.

Score | Description
-----:|:-----------
0 | Oh oh. Now is a good time to take a look at PSIP (see below) for identifying and tracking practices that could be used or improved.
<10 | Good start! A process improvement strategy such as PSIP (see below) could be a good way to get you to the next level.
10-100 | Cool! Adopting advanced practices can be challenging without a process improvement strategy such as PSIP (see below.).
100-400 | Impressive! Seems like you have really good practices already in place. Have you thought about how you could improve from here?
\>400 | Wow, you rock! Would you be interested in writing a blog article on your software engineering practices?

### Where To Go Next?

Regardless of your score, there is always room for improvement. One way to improve your project’s practices is to look at a software improvement strategy, such as the Productivity and Sustainability Improvement Planning (PSIP). PSIP is a lightweight process that uses Progress Tracking Cards (PTCs) to track the improvements you are making. For more information, see <https://bssw.io/psip>.

If you and your team would like assistance from a PSIP IDEAS-ECP facilitator in rating your project, starting PSIP, and creating a project tracking card (PTC), contact us at <https://bssw.io/contact>.

<div style='page-break-after:always'></div>

## Project Self-Survey

The form below shows a range of practices that increase in maturity. Check the practices that your project already uses, score each basic practice as 1 point, intermediate as 10 points and advanced as 100 points. Write the score in the box below.

If you and your team would like assistance from a PSIP IDEAS-ECP facilitator in rating your project, starting PSIP, and creating a project tracking card (PTC), contact us at <https://bssw.io/contact>.

### Better Development

1.  Revision Control

    - <input type="checkbox" class="survey" value="1"> Uses revision control system such as Git [1 point]
    - <input type="checkbox" class="survey" value="10"> Uses a basic development workflow (e.g., basic Git workflow) [10 points]
    - <input type="checkbox" class="survey" value="100"> Uses an advanced development workflow (e.g., Gitflow) [100 points]

2.  Code Reviews

    - <input type="checkbox" class="survey" value="1"> Ad-hoc code reviews [1 point]
    - <input type="checkbox" class="survey" value="10"> Regular code reviews (e.g., weekly meetings) [10 points]
    - <input type="checkbox" class="survey" value="100"> Code reviews automated in workflow (e.g., via pull requests) [100 points]

3.  Issue Tracking

    - <input type="checkbox" class="survey" value="1"> Manual issue tracking via email or other medium [1 point]
    - <input type="checkbox" class="survey" value="10"> Dedicated issue tracking system being used [10 points]
    - <input type="checkbox" class="survey" value="100"> Integrated issue tracking  (e.g., pull requests) [100 points]

4.  Deployment

    - <input type="checkbox" class="survey" value="1"> Manual deployment using a script [1 point]
    - <input type="checkbox" class="survey" value="10"> Deployment as part of development workflow with manual intervention [10 points]
    - <input type="checkbox" class="survey" value="100"> Continuous deployment [100 points]

5.  Documentation

    - <input type="checkbox" class="survey" value="1"> Ad-hoc text files [1 point]
    - <input type="checkbox" class="survey" value="10"> Code and documentation are cross referenced and updated when committed to repository [10 points]
    - <input type="checkbox" class="survey" value="100"> Integrated with the package release workflow [100 points]

### Better Planning

1.  Development Process

    - <input type="checkbox" class="survey" value="1"> Has development process but it is based on ad-hoc rules [1 point]
    - <input type="checkbox" class="survey" value="10"> Employs an iterative development process [10 points]
    - <input type="checkbox" class="survey" value="100"> Uses an agile development methodology [100 points]

2.  Due Diligence

    - <input type="checkbox" class="survey" value="1"> Formal guidelines for accepting contributions [1 point]
    - <input type="checkbox" class="survey" value="10"> Clearly defined standards for coding and documentation [10 points]
    - <input type="checkbox" class="survey" value="100"> Provenance and license checking for contributions [100 points]

3.  Software Design

    - <input type="checkbox" class="survey" value="1"> Development guidelines include design in the process [1 point]
    - <input type="checkbox" class="survey" value="10"> A modeling language is employed for key aspects of the project [10 points]
    - <input type="checkbox" class="survey" value="100"> Visual modeling using a graphical representation to capture design [100 points]

4.  Onboarding

    - <input type="checkbox" class="survey" value="1"> Initial onboarding process is documented [1 point]
    - <input type="checkbox" class="survey" value="10"> Used for supervisors for new hires [10 points]
    - <input type="checkbox" class="survey" value="100"> Used for all personnel changes [100 points]

5.  Requirements Analysis

    - <input type="checkbox" class="survey" value="1"> Development guidelines include requirements gathering [1 point]
    - <input type="checkbox" class="survey" value="10"> Formal requirements gathering is undertaken as part of the project [10 points]
    - <input type="checkbox" class="survey" value="100"> Requirements management process is employed [100 points]

### Better Reliability

1.  Testing

    - <input type="checkbox" class="survey" value="1"> Comparison used to create system-level no-change tests [1 point]
    - <input type="checkbox" class="survey" value="10"> Unit testing for refactored and new code [10 points]
    - <input type="checkbox" class="survey" value="100"> Continuous integration [100 points]

2.  Reproducibility

    - <input type="checkbox" class="survey" value="1"> Publication of code [1 point]
    - <input type="checkbox" class="survey" value="10"> Inclusion of data when code is published [10 points]
    - <input type="checkbox" class="survey" value="100"> Automatic provenance capture system is employed [100 points]

### Score <span id="survey-total" style="text-decoration:underline;">0</span>

*Be sure to print this page out for your records!* We do not save your data in any way.
