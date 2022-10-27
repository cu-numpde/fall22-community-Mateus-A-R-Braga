# Community Software Analysis Proposal
Please edit this file and push to your repository.

## Software: Clawpack

Clawpack stands for Conservation Laws Package. Clawpack is a collection of solvers for linear and nonlinear hyperbolic systems of conservation laws, such as advection or acoustic type problems. Aimed at solving conservation laws, Clawpack naturally employs the finite volume method. The collection includes classic Clawpack: a general hyperbolic PDE solver (written in Fortran), AMRClaw: with adaptive mesh refinement (written in Fortran), GeoClaw: aimed at geophysical flow (written in Fortran), and PyClaw: a version of Clawpack written in Python. Applications sutiable for the suite of Clawpack solvers includes variable-coefficient advection, acoustics, Euler equations, and many more conservation problems. The primary audience varies depending on which solver is used from the collection. In general, Clawpack could be useful to those who study high speed flows because the package was designed to handle hyperbolic equations. Specifically for Geoclaw, it is well suited for people interested in solving geophysics problems.

The key features of the software include: 
* Capability to solve general hyperbolic partial differential equations (PDEs)
    * Riemann solvers for many common applications are bundled with the software
    * A Riemann solver needs to be provided to deal with discontinuities (shocks) at the faces between cells
* AMRClaw and GeoClaw includes adaptive mesh refinement (AMR)
* PyClaw allows for parallelism scalable to the tens of thousands of cores

Summary list of solvers included with Clawpack:
* Classic (single grid solvers in Fortran)
* AMRClaw Description and Detailed Contents (adaptive mesh refinement in Fortran)
* GeoClaw Description and Detailed Contents (geophysical flows with AMR, in Fortran)
* PyClaw (Python version of solvers)



### Stats

| Description | Your answer |
|---------|-----------|
| Repository URL |  https://github.com/clawpack/clawpack  |
| Main/documentation website |  http://www.clawpack.org/  |
| Year project was started |  1994  |
| Number of contributors in the past year | 3 |
| Number of contributors in the lifetime of the project | 20 major contributors |
| Number of distinct affiliations | >10 |
| Where do development discussions take place? | Slack, claw-dev Google group (http://groups.google.com/group/claw-dev/), issue trackers on Github, Gitter, Twitter, claw-users Google group |
| Typical number of emails/comments per week? |  Last conversation in claw-dev Google group was August 28, 2022 (2 months ago) |
| Typical number of commits per week? | Last commit was 2 months ago |
| Typical commit size | Approximately 100-200 additions/deletions per commit (over the past year) |
| How does the project accept contributions? | pull requests  |
| Does the project have an automated test suite? | yes |
| Does the project use continuous integration? | yes |
| Are any legal/licensing steps required to contribute? | No |

### Install and run

Check the following boxes when complete or add a note below if you
encountered a problem.

- [x] I have installed the software
- [x] I have run at least one example
- [x] I have run the test suite
- [ ] The test suite passes

### Notes/concerns/risks

Please comment on any anomalies or known risks to following this
project, if you were unable to answer any questions above, or
otherwise have concerns about the appropriateness of the software.  If
the project requires a contributor license agreement or other
procedural steps, please explain here.  "None at this time" is
acceptable for this question.

Notes:

* The Pyclaw is the most active and has the most documentaiton and suport.
    * this would be the best for a project.

* If using either the Fortran or Python installations there is an automated test suite that runs several tests and compares the solution (parts of the soltution) to archived resutls.

* For PyClaw 46 of 48 tests in the test suite pass and two tests fail with an error that there is no such file or directory for the verification file (the file name for the verificaiton file might be mislabeld for those tests)

* For the Fortran based tests all three tests in the test suite fail.

* Permissive license: Berkeley Software Distribution (BSD) license (BSD 3-Clause)
    * Concern about license: On the Clawpack website the copyright is from 1994-2020, does that mean it is no longer in effect? => "Copyright (c) 1994–2020, The Clawpack Development Team. All rights reserved."

* Travis continuos integration is used 

* Submitted request to join Clawpack Slack. Have yet to hear back from them.

* In the docs directory (after installing) there are no files

* Seemed most active approximately 5-10 years ago, less active these days
    * May not be the best choice going forward for a project

#### Note on copyright
Students retain copyright on any work done in completion of a CU
course, so you are authorized to sign a [contributor license
agreement (CLA)](https://en.wikipedia.org/wiki/Contributor_License_Agreement),
affirm a [developer's certificate of
origin (DCO)](https://en.wikipedia.org/wiki/Developer_Certificate_of_Origin),
etc.  If you have concerns about this, please note them and/or reach
out to Jed directly.
