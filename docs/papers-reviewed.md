# Papers that where reviewed

## Template

Table columns of template:

* Paper_id: paper id in the list below, for example ID = 11 for the first paper.
* Name: name of criteria.
* Definition: description/summary of the criteria.
* Qualitative/quantitative: if the criteria is objective/measurable (possible to automate) or subjective and difficult to automate.
* Targeted to SW (see <https://github.com/eosc-sq/overleaf-ensure-sq/blob/main/landscaping.tex>): at the, moment one of:
  * Library
  * Framework
  * Application (such as Monte-Carlo simulation)
  * Analysis script
  * Services and platforms
* Reviewer(s): reviewer short name, for example DG for Daniel Garijo, see below.
* Comment: any other comment the reviewer sees fit to make.

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
|          |       |            |                          |                |           |         |

## Reviewers

* DG - Daniel Garijo
* ER - Elisabetta Ronchieri
* JC - Leyla Jael Castro
* LC - Laura del Cano
* MC - Miguel Colom
* MD - Mario David
* MT - Massimo Torquati
* MV - Maxime Van den Bossche
* VL - Violaine Louvet
* IC - Isabel Campos
* CL - Cerlane Leong

## 11 - Software quality through the eyes of the end-user and static analysis tools: A study on Android OSS applications

Srisopha K., Alfayez R.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-85051522416&doi=10.1145%2f3194095.3194096&partnerID=40&md5=7a9dc5d4116e134e2a85128cb3328d90>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 11       | Code complexity      |  Paper does not provide a definition, but the less complex the code is, the better          |  Quantitative  | all types | DG        | See below    |
| 11       | Number of code smells      |  certain structures in the code which indicate a violation of fundamental design principles. The lower code smells, the better. Ref: Martin Fowler and Kent Beck. 1999. Refactoring: improving the design of existing code. Addison-Wesley Professional.  | Quanticative | all types | DG        | See below    |
| 11       | Comment density      | The idea here is that better commented code is easier to understand | Quantitative  | all types | DG        | See below    |
| 11       | User reviews      | The paper attempts to find correlation between user reviews and code quality. However, "to some extent, having high or low code quality does not necessary ensure user satisfaction" | Quantitative | apps with a store | DG        | See below    |
| 11       | PMD quality metrics     | Empty code, Naming, Braces, Import statements, Coupling, Unused Code, Unnecessary, Design, Optimization, String and StringBuffer | Quantitative | apps with a store | DG        | See below    |
| 11       | Findbugs quality metrics      | Dodgy code, Bad practice, Malicious code, Performance, Correctness, Security, Multithreaded correctness, Internalization | Quantitative | apps with a store | DG        | See below    |

**Quality Model** ("is based on", "mentions"): ISO/IEC 25010

This paper proposes a quality analysis from an empirical point of view. It uses three tools for quantitative analysis: SonarQube, PMD and FindBugs. The quality metrics are not proposed per se in the paper, but are useful candidates.

The paper mentions ISO/IEC 25010 software product quality characteristics. These are:

* functional suitability
* performance efficiency
* usability
* portability
* compatibility
* reliability
* maintainability
* security

The following table shows how each tool tackles different metrics. However, some are not defined:

|Abbr.| Tool      | Metric|
|:---:|:---------:|:-----:|
| CS  | SonarQube | Number of code smells|
| PD  | PMD       | Empty code, Naming, Braces, Import statements, Coupling, Unused Code, Unnecessary, Design, Optimization, String and StringBuffer|
| FB  | FindBugs  | Dodgy code, Bad practice, Malicious code, Performance, Correctness, Security, Multithreaded correctness, Internalization|

## 41 - Fostering software quality assessment

Brandtner M.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-84886382849&doi=10.1109%2fICSE.2013.6606725&partnerID=40&md5=9e042076903be6351b3b97be6a877cb3>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 41       | Individual Information | Stakeholder's information influenced by the role involved and the type of software. |  Qualitative  |  All  | ER | Type of software can be rich client, web application and so on. |
| 41       | Stakeholder context | Detail e.g. stakeholder role and tool-usage data by each stakeholder |  Qualitative |  All | ER        |  Software architects, developers and testers are the considred essential role in the development process. |
| 41       | Technical context | Information about the source code by using e.g. software metrics |  Quantitative |  All | ER        |  Type of software can be rich client, web application and son. |
| 41       | Context-sensitive | The relation between the data, the world the data refers to, and the observer's expectations, intentions and interests |  Qualitative |  All | ER        |  The paper provides an illustrative example to support different stakeholders in the quality assessement of a software system. |

**Quality Model** ("is based on", "mentions"):

**NOTE: This article is mainly on software quality assessment than software quality definition.** However it contains an interesting approach based on stakeholder's information needs and the tailoring of information for software quality assessment. This paper also provides some guidelines to support the activities carried out by each type of stakeholders.


## 45 - A systematic review of quality attributes and measures for software product lines

Montagud S., Abrahão S., Insfran E.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-84865626740&doi=10.1007%2fs11219-011-9146-7&partnerID=40&md5=33b25cd0a25fc09685e06cbc9c988f14>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
 | 45 | Binary size | Binary size | Quantitative |  | JC | Exclude, not sure how good this criterion is |
 | 45 | Complexity of the source code | Cyclomatic complexity | Quantitative |  | JC |  |
 | 45 | Performance |  | Quantitative |  | JC |  |
 | 45 | Complexity of the source code (for classes and components) |  | Quantitative |  | JC | Requires well established software engineering practices.  Alternative: Yes/No and how (e.g., code review) |
 | 45 | Complexity of diagrams (for classes and components) |  | Quantitative |  | JC | Requires well established software engineering practices. Alternative: Yes/No and how (e.g., some sort of peer-review) |
 | 45  | Complexity of an architecture |  | Quantitative |  | JC | Requires well established software engineering practices. Alternative: Yes/No and how (e.g., some sort of peer-review) |
 | 45 | Complexity of a use case |  | Quantitative |  | JC | Requires well established software engineering practices. Alternative: Yes/No and how (e.g., some sort of peer-review) |
 | 45 | Complexity of a use case diagram |  | Quantitative |  | JC | Optional, not sure use case diagrams are always needed. Exclude |
 | 45 | Maintainability Index (MI) (for the whole, for a component, for the architecture |  | Quantitative |  | JC |  |
 | 45 | Reusability (of the whole and the components) |  | Quantitative |  | JC |  |
 | 45 | Reusability of the architecture |  | Quantitative |  | JC |  |
 | 45 | Applicability |  | Quantitative |  | JC | Validation against use cases or requirements (?) |
 | 45 | Understandability |  | Quantitative |  | JC |  |
 | 45 | Efficiency |  | Quantitative |  | JC | Exclude (difficult to measure) |
 | 45 | Effort required for changes |  | Quantitative |  | JC | Exclude (difficult to measure) |
 | 45 | Size (of modules, lines, components) |  | Quantitative |  | JC | Exclude, not sure how good this criterion is |
 | 45 | Maturity | Time for the code to fail, number of resolved bugs, number of open bugs | Quantitative |  | JC |  |
 | 45 | Configuration Complexity |  | Quantitative |  | JC | Configuration to run the code (?) |
 | 45 | Modularity of the architecture |  | Quantitative |  | JC |  |
 | 45 | Customizability |  | Quantitative |  | JC | Exclude, looks like related to customization by final user |
 | 45 | Internal cohesion |  | Quantitative |  | JC | Exclude (difficult to measure). Requires well established software engineering practices |
 | 45 | Coherence |  | Quantitative |  | JC | Exclude (difficult to measure). Requires well established software engineering practices |

**Quality Model** ("is based on", "mentions"):

## 46 - Standardized code quality benchmarking for improving software maintainability

Baggen R., Correia J.P., Schill K., Visser J.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-84860465895&doi=10.1007%2fs11219-011-9144-9&partnerID=40&md5=042a7624f2cb95e1a97643ef8e0f9071>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 46       | Volume | Size of the software application | Quantitative | All Types | LC        | Estimated rebuild value |
| 46       | Redundancy | Level of redundancy in code | Quantitative | All Types | LC        | Percentage of redundant code |
| 46       | Unit size | Lowel-level piece of functionality that should be maintained | Quantitative | All Types | LC        | Lines of code per unit (Unit=smallest piece of invokable code) code |
| 46       | Unit complexity | Of the software application | Quantitative | All Types | LC        | Cyclomatic complexity per unit |
| 46       | Unit interface size | Number of parameters in interface | Quantitative | All Types | LC        | Number of parameters per unit |
| 46       | Module coupling |  | Quantitative | All Types | LC        | Number of parameters per unit | Number of incoming calls per module |

**Quality Model** ("is based on", "mentions"): ISO/IEC 9126

The paper presents a standardized measurement model based on the ISO/IEC 9126 definition of maintainability and source code metrics.
In this ISO standard they propose a hierarchical quality model made of quality characteristics decomposed in subcharacteristics.
They choose 6 code properties as key metrics for the quality assessment of the subcharacteristics.
Then they keep a benchmark database to perform comparison and evaluate new measurements. In this database they use metadata attributes to tag each measurement and help with comparing.

The quality characteristics from ISO/IEC 9126 they mention are:

* Analysability: measured with Volume, Redundancy and Unit size.
* Changeability: measure with Redundancy, Unit complexity and Module coupling.
* Stability: measured with Unit inteface size and Module coupling.
* Testability: measured with Unit complexity and Unit size.

## 58 - Quality specification and metrication, results from a case-study in a mission-critical software domain

Trienekens J.J.M., Kusters R.J., Brussel D.C.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-77956057048&doi=10.1007%2fs11219-010-9101-z&partnerID=40&md5=8676a4867b80d63fce5b0d10d732fb63>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 58 | real-time performance |  | Quantitative | critical systems (non exclusive) | MC |  |
| 58 | reliability | mission specific | Quantitative | critical systems (non exclusive) | MC |  |
| 58 | consistency | same rules along SW development process | Quantitative | | MC |  |
| 58 | transparency | | Quantitative | | MC |  |
| 58 | usability | feedback from final users | Qualitative | | MC |  |
| 58 | effectiveness | useful for final users | Quantitative | | MC |  |
| 58 | productivity | fast results from final users | Quantitative | | MC |  |
| 58 | usability | easy to use by final users | Quantitative | | MC |  |
| 58 | safety |  not prone to error by final users | Quantitative | | MC |  |
| 58 | satisfaction |  feedback from final users | Qualitative | | MC |  |
| 58 | maintainability |  Easy to modify according to changing needs | Quantitative | | MC |  |
| 58 | portability | Easy to implement in different scenarios | Quantitative | | MC |  |

**Quality Model** ("is based on", "mentions"):

## 85 - Achieving quality in open-source software

Aberdour M.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-33846917203&doi=10.1109%2fMS.2007.2&partnerID=40&md5=08d47741430e05c8a0ceb015a1f43a04>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 85       | Code documentation | The code is documented      | Qualitative and quantitative | all types | DG        | See below |
| 85       | Sustainable community | Is there an active community behind the software product? (i.e., for maintenance/bug fixing) | both |  all types              | DG        | See below |
| 85       | Code modularity   | The code of the project is not a whole entity, but is fragmented in smaller modulues that make it easier to contribute to | Quantitative | all types | DG        | See below |
| 85       | Code goes through code reviews/peer review | Each contribution is assessed by a contributor different from the author |  Qualitative                        | All types  | DG        | See below |
| 85       | Tests | Each method/function has a test to support it | Quantitative | all types | DG        | See below |
| 85       | Tutorials | Availability of material explaining how to use the target software through examples | Qualitative/Quantitative | All types  | DG        | See below |

**Quality Model** ("is based on", "mentions"):

The paper focuses on project management for quality, comparing open source software projects with non open initiatives.

* Quality areas: quality assurance (focuses on process and procedure, learning from mistakes, and ensuring good management practice) and quality control (process of verification and validation)

## 88 - Driving software quality: How test-driven development impacts software quality

Crispin L.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-33846907119&doi=10.1109%2fMS.2006.157&partnerID=40&md5=1c6ac14fdd83073f861f9ec5b1e95701>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 88       | Test driven development | Definition and development of unit tests for each functionality | Quantitative | All | ER |  |
| 88       | Project creole      | A shared language (between manager and developers)           | Qualitative: managers can improve the way they define features, developers can easily produce well-tailored program  | All | ER | It considers important the development of a shared language or project creole between business people and developers to find some common ground and work together in order to improve software development.  |

**Quality Model** ("is based on", "mentions"):

**NOTE: this is a paper of 2 pages**. For my point of view it can be left out for quality definition. 

## 93 - Early estimation of software quality using in-process testing metrics: A controlled case study

Nagappan N., Williams L., Vouk M., Osborne J.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-77955433687&doi=10.1145%2f1083292.1083304&partnerID=40&md5=c3b21a87b407b65539153ab3017b0eda>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 93       | Test quantification SM1 | Number of Assertions SLOC* | Quantitative | Java code | LC        | Accounts for coding/testng style |
| 93       | Test quantification SM2 | Number of Test Cases SLOC* | Quantitative | Java code | LC        | Accounts for coding/testng style |
| 93       | Test quantification SM3 | Number of Assertions divided by Number of Test Cases | Quantitative | Java code | LC        | Accounts for coding/testng style |
| 93       | Test quantification SM4 | (TLOC/SLOC*)  divided by (Number of Classes Test Number of ClassesSource) | Quantitative | Java code | LC        | Serves as a control measure to counter the confounding effect of class size |
| 93       | Cyclomatic complexity | Relative ratio of test to source code in Cyclomatic Complexity | Quantitative | Java code | LC        | Complexity and O-O metrics |
| 93       | CBO  | Relative ratio of test to source code in Coupling between objects | Quantitative | Java code | LC        | Complexity and O-O metrics |
| 93       | DIT  | Relative ratio of test to source code in Depth of Inheritance | Quantitative | Java code | LC        | Complexity and O-O metrics |
| 93       | WMC  | Relative ratio of test to source code in  weighted methods per class | Quantitative | Java code | LC        | Complexity and O-O metrics |
| 93       | Relative size adjustment  | SLOC* divided by Minimum SLOC* | Quantitative | Java code | LC        | Complexity and O-O metrics |

**Quality Model** ("is based on", "mentions"):

\* Source Lines of Code (SLOC) is computed as non-blank, non-comment source lines of code

\+ Test Lines of Code (TLOC) is computed as non-blank, non-comment test lines of code

They present a metric suite called the Software Testing and Reliability Early Warning metric suite for Java (STREW-J) that can be used as an early indication of an external measure of software application quality. They put a greater emphasis on internal software metrics, particularly those involving the testing effort. It requires the existence of an extensive suite of automated unit test cases being created as development proceeds.

## 99 - The evolution path for industrial software quality evaluation methods applying ISO/IEC 9126:2001 quality model: Example of MITRE's SQAE method

Côté M.-A., Suryn W., Laporte C.Y., Martin R.A.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-17444388547&doi=10.1007%2fs11219-004-5259-6&partnerID=40&md5=09ec05c221610b4c799ab6111def6568>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: | 
| 99 | consistency | in many aspects of ISO/EIC 9126 | Quantitative | | MC |  |
| 99 | independence | interoperativity, changeability, adaptability | Quantitative | | MC |  |
| 99 | modularity | changeability, testability | Quantitative | | MC |  |
| 99 | documentation | learnability, analysability | Quantitative | | MC |  |
| 99 | self-descriptiveness | understandability, operability, analysability | Quantitative | | MC |  |
| 99 | anomaly-control | maturity, fault tolerance, recoverability, reliability compliance | Quantitative | | MC |  |
| 99 | design simplicity | security, analysability, changeability, stability, testability | Quantitative | | MC |  |

**Quality Model** ("is based on", "mentions"): ISO/IEC 9126

Mainly a correlation between their proposed quality factors and the sub-characteristics in ISO/EIC 9126.

## 108 - Construction of a systemic quality model for evaluating a software product

Ortega M., Pérez M., Rojas T.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-3543054780&doi=10.1023%2fA%3a1025166710988&partnerID=40&md5=f6915840807fb5204c5c331644d47524>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 108      | Systemic model | Extends ISO9126, Dromey and McCall models  |  Mainly qualitative: set of measures and practices   |   all   | MT   | See below     |

**Quality Model** ("is based on", "mentions"): Extends ISO9126, Dromey and McCall models

Comment

The study proposes a systemic quality model. Authors developed a process framework with which to evaluate product quality considering the processes that contribute to product
quality. They basically extend ISO 9126 product quality model considering the roles of stakeholders (project managers, developers, and users) trying to evaluate the internal quality,
which includes functionality, reliability, usability, efficiency, maintainability, and portability characteristics. Authors claimed that those quantities relate to each other and must
be integrated for a systemic global quality design. The work does not analyze the effect of the method applied on different stakeholders.

## 129 - Controlling and predicting the quality of space shuttle software using metrics

Schneidewind N.F.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-0343935307&doi=10.1007%2fBF00404649&partnerID=40&md5=b99281a03e36e4acaf4ca5067792314f>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 129      | eta1 | Unique operator count | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | eta2 | Unique operand count | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | n1 | Total operator count | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | n2 | Total operand count | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | stms | Total statement count (executable code; no comments) | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | loc | Total non-commented lines of code | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | comments | Total comment count | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | nodes | Total node count (in control graph) | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | edges | Total edge count (in control graph) | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | paths | Total path count (in control graph) | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | cycles | Total cycle count (in control path) | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | maxpath | Maximum path length (edges in control path) | Quantitative           | Space SW written in HAL/S | LC        |         |
| 129      | avepath | Average path length (edges in control graph) | Quantitative           | Space SW written in HAL/S | LC        |         |

**Quality Model** ("is based on", "mentions"):

This is a very old paper that tries to relate quality measurements at development time with quality predictions for production. It is only valid for a specific software used in the space shuttle.

## 140 - Modelling software quality in the commercial environment

Gillies A.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-0001332319&doi=10.1007%2fBF01720924&partnerID=40&md5=a0b468b060b629ea3ced5fefac2c2848>

| Paper_id | Name       | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :--------: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 140 | Reliability     | How often does it go wrong? How long is it unavailable? Is any information lost at recovery?                           | Quantitative | | MD | SW in operation |
| 140 | Efficiency      | The critical resources needed by the operator to carry out the critical tasks can be monitored                         | Quantitative | | MD | SW in operation |
| 140 | Security        | Measured as the resource cost expended to solve problems caused by unauthorized activity                               | Quantitative | | MD | SW in operation |
| 140 | Integrity       | Measured as the resource cost expended to solve problems caused by inconsistencies within the system                   | Quantitative | | MD | SW in operation |
| 140 | Usability       | Measured using user surveys. may also be assessed in terms o f calls upon support staff                                | Quantitative | | MD | SW in operation |
| 140 | Maintainability | Measured by the resources expended in terms o f time and cost in keeping a system up and running over a period of time | Quantitative | | MD | SW in operation |
| 140 | Adaptability    | Measured in the same way as maintainability, i.e. by the resources expended in adapting the system to meet new requirements over a period of time | Quantitative | | MD |  |
| 140 | Portability     | Measured according to Gilb's measure | Quantitative | | MD | see below |
| 140 | Timeliness      | Assessed in terms of the costs of non-delivery | Quantitative | | MD |  |
| 140 | Cost~Benefit efficiency | measured in simple financial terms. The costs of installing and maintaining the system are weighed against the assessment of business benefits | Quantitative | | MD |  |
| 140 | Ease of transition | Assessed in terms o f staff time expended. The effectiveness of transition may be assessed in terms of the quality of the resulting system particularly the area of integrity. | Quantitative  | | MD | SW in operation |
| 140 | Userfriendliness   | Measured in terms of the effect upon the effectiveness of the user. The measure of user friendliness in business terms is the productivity of the user. | Quantitative | | MD | SW in operation |

**Quality Model** ("is based on", "mentions"):

* Watts, R. (1987) Measuring Software Quality, NCC Publications Manchester.
* Gilb, T. (1988) Principles of Software Engineering Management, Addison-Wesley.

* *MD* - How different parties/stakeholders perceived a given Quality Model:
  * Analysis of Structured interviews to people from 6 different market sectors, and see how they
    interpret a set of quality attributes.
  * Attributes suggested by the author and based mainly on:
    * Watts, R. (1987) Measuring Software Quality, NCC Publications Manchester.
    * Gilb, T. (1988) Principles of Software Engineering Management, Addison-Wesley.
    * Measured in general in terms of costs of Resources (Human and Infrastructure).
  * Portability according to Gilb: P = 1 - (ET/ER)
    * P represents portability
    * ET effort required to transfer the system to a new environment
    * ER represents the effort required to establish the system in its existing environment.

## 144 - Practice of quality modeling and measurement on software life-cycle

Hirayama Masayuki, Sato Hiroyuki, Yamada Atushi, Tsuda Junichiro

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-0025022794&partnerID=40&md5=155e3e9926c8e675616e8d839798a6e1>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 144      | ESQUT | It is a source code quality index  |  Quantitative            |  (old) C code  | MT        | See below  |

**Quality Model** ("is based on", "mentions"):

The paper's main motivation is that Halstead's and McCabe's metrics are not practical and have some limitations (in the case of programs with GOTO statements and deep nesting). The authors propose a new quantitative metric called ESQUT-C (for C programs) considering:

* n. of GOTO statements
* n. of module exits
* n. of conditional statements
* n. of procedure blocks
* nesting level of procedure blocks
* number of executions
* number of lines (LOC)
* number of real digits

They also showed how those metrics correlate with McCabe's and Halstead's metrics.
The paper has been published in 1990.

## 146 - Quantitative evaluation of software quality

Boehm B.W., Brown J.R., Lipow M.

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-85042377749&partnerID=40&md5=86df793c94725cf352a0b8b3d8227c3c>

| Paper_id |           Name            |                          Definition                          | Qualitative/Quantitative | Targeted to SW | Reviewer |                           Comment                            |
| :------: | :-----------------------: | :----------------------------------------------------------: | :----------------------: | :------------: | :------: | :----------------------------------------------------------: |
|   146    |       ACCESSIBILITY       |           facilitates selective use of its parts.            |                          |      All       |    VL    | Necessary for efficiency, testability and human engineering  |
|   146    |      ACCOUNTABILITY       | its usage can be measured; critical segments of code can be instrumented with probes to measure timing, whether specified branches are exercised, etc. |       Quantitative       |      All       |    VL    |                                                              |
|   146    |         ACCURACY          | its outputs are sufficiently precise to satisfy their intended us |       Quantitative       |      All       |    VL    |                  Necessary for reliability                   |
|   146    |      AUGMENTABILITY       | it can easily accommodate expansion in component computational functions or data storage requirements |                          |      All       |    VL    |                 Necessary for modifiability                  |
|   146    |     COMMUNICATIVENESS     | it  facilitates the specification of inputs and provides outputs whose form and content are easy to assimilate and useful. |                          |      All       |    VL    |       Necessary for testability and human engineering        |
|   146    |       COMPLETENESS        | all its parts are present and each part is fully developed.  |       Quantitative       |      All       |    VL    | External references are available and required functions are coded and present as designe |
|   146    |        CONCISENESS        |            excessive information is not present.             |       Quantitative       |      All       |    VL    | Programs are not excessively fragmented nor the same sequence of code is repeated in numerous place ... |
|   146    |        CONSISTENCY        | it contains uniform notation, terminology and symbology within itself |       Quantitative       |      All       |    VL    |        Coding standards are homogeneously adhered to         |
|   146    |    DEVICE-INDEPENDENCE    | it can be executed on computer hardware configurations other than its current on |       Quantitative       |      All       |    VL    |                  Necessary for portability                   |
|   146    |        EFFICIENCY         |     it fulfills its purpose without waste of resources.      |       Quantitative       |      All       |    VL    |              Choice of efficient algorithm ...               |
|   146    |     HUMAN ENGINEERING     | it fulfills its purpose without wasting the users' time and energy, or degrading their morale |       Qualitative        |      All       |    VL    |   Implies accessibility, robustness and communicativeness    |
|   146    |        LEGIBILITY         |     its function is easily discerned by reading the code     |       Qualitative        |      All       |    VL    |               Necessary for understandability                |
|   146    |      MAINTAINABILITY      | it facilitates updating to satisfy new requirements or to correct deficiencies. |                          |      All       |    VL    |         Code understandable, testable and modifiable         |
|   146    |       MODIFIABILITY       | it facilitates the incorporation of changes, once the nature of the desired change has been determined |                          |      All       |    VL    |                                                              |
|   146    |        PORTABILITY        | it can be operated easily and well on computer configurations other than its current one. |       Quantitative       |      All       |    VL    |             Use of standard library function ...             |
|   146    |        RELIABILITY        | it can be expected to perform it s intended functions satisfactorily |                          |      All       |    VL    | The program will compile, load and execute, producing answers of the requisite accuracy |
|   146    |        ROBUSTNESS         | it can continue to perform despite some violation of the assumptions in its specification |       Quantitative       |      All       |    VL    | The program will properly handle inputs out of range or in different format ... |
|   146    |    SELF-CONTAINEDNESS     | it performs all its explicit and implicit functions within itself . |                          |      All       |    VL    | Example of implicit functions : initialization, input checking ... |
|   146    |   SELF-DESCRIPTIVENESS    | it contains enough information for a reader to determine or verify its objectives, assumptions, constraints, inputs, outputs, components, and revision status. |       Qualitative        |      All       |    VL    |       Necessary for testability and understandability        |
|   146    |      STRUCTUREDNESS       | it possesses a definite pattern of organization of its interdependent parts. |       Qualitative        |      All       |    VL    |   Standard control structure have been followed in coding    |
|   146    |        TESTABILITY        | it facilitates the establishment of verification criteria and supports evaluation of its performance. |       Quantitative       |      All       |    VL    | requirements are match to specific modules or diagnostics capabilities are provided |
|   146    |     UNDERSTANDABILITY     |            its purpose is clear to the inspector.            |       Qualitative        |      All       |    VL    | Names are used consistently, modules are self-descriptive, ... |
|   146    | USABILITY (AS-lS UTILITY) |       it is reliable, efficient and human-engineered.        |                          |      All       |    VL    | The function performed by the program is useful elsewhere, is robust against human errors or does not require excessive core memory... |

**Quality Model** ("is based on", "mentions", "defines"): define Boehm software quality model

The article describe the Boehm software quality model. It identifies characteristics of quality structured in a tree (see above for this characteristics). It also gives a few example of quality metrics (Boehms wrote a book on the subject). It also explains the link between the identification of types of error and when they appear during the software life-cycle and at which phase of the cycke they are corrected. It shows that early application of automated and semiautomated consistency, robustnes and self containedness checkers leads to significant improvements in software error detection. It gives some input on quality-enhancing tools and techniques. Life cycle activities with significant effects on software quality:

* setting software quality objectives and priorities
* performing software quality benchmarking
* using software quakity checklists
* establishing an explicit quality assurance activity
* using machine-analyzable software specifications
* ensuring testable software requirements
* using a requirements-properties matrix
* establishing standards
* using an automated code auditor for standards compliance
* performing design and code inspections

## 118 - A critical look at ISO 9000 for software quality management

Stelzer D., Mellis W., Herzwurm G.


<https://www.scopus.com/inward/record.uri?eid=2-s2.0-0642363924&doi=10.1023%2fA%3a1018591430752&partnerID=40&md5=9181348bb75865be23649ef29338594f>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 120       | Individual Information | Impact of ISO 9000 on software development: a survey |  Qualitative |  All  | IC | Critical analysis of ISO 9000 as regard to its implications in software development processes in companies |
| 120       | Stakeholder context | Managerial layers, programmers, ISO auditors |  Qualitative |  All | IC        |  Distinguises between programmers context and managerial layer|
| 120       | Technical context | analysis of the feedback received from companies certified with ISO 9000 |  Qualitative |  All | IC        |  Type of software can be anything |
| 120       | Context-sensitive | The relation between the actors involved in the certification ISO 9000 evaluation and management |  Qualitative |  All | IC        |  The paper provides a useful description of the problems software developers may go through when ISO 9000 is implemented |

**Quality Model** ("is based on mentions")

**NOTE: This article is mainly on context definition and its role in the process of software quality evaluation** 

This article describes the impact on software quality management as reported by several organiztions that have an ISO9000 certification. What has been the impact
in the quality management of their software that can be attributed to being certified ISO 9000. The survey was centered in five elements: code reviews and inspections,
software testing, product and process measurements, measurement of quality cost and demonstrations of quality improvement. Most critics are around the lack of real 
impact in the time-to-market strategies for software products, and to the burden they generate to the developers due to the exceisve "top-down approach" and 
centralized management quality management approach of the ISO 9000 system. Excesive load of documentation production for auditing purposes is also a problem 
reported by the companies involved in the analysis. Aspects such as moral and motivation of the programmers are not considered. 



## 120 - Specifying software quality with the extended ISO model

R.H.J. van Zeist and P.r.H. Hendriks

<https://www.scopus.com/inward/record.uri?eid=2-s2.0-27144550799&doi=10.1007%2fBF00209185&partnerID=40&md5=64394714677ede47867fcd1a5625efff>

| Paper_id | Name  | Definition | Qualitative/Quantitative | Targeted to SW | Reviewer  | Comment |
| :------: | :---: | :--------: | :----------------------: | :------------: | :-------: | :-----: |
| 120       | Individual Information | Aligning the specification on what means software quality |  Qualitative |  All  | IC | Extension to the ISO 9126 model, superseed later by ISO/IEC 25010 in year 2011 |
| 120       | Stakeholder context | End users, developers and evaluator |  Qualitative |  All | IC        |  Distinguises between user context and developer context to gather quality requirements and adds an evaluator context |
| 120       | Technical context | Information about the source code asking about perceptions beyond technical functionalities such as user-friendliness, etc... |  Qualitative |  All | IC        |  Type of software can be any |
| 120       | Context-sensitive | The relation between the different actors involved in the software lifecycle, from developers to maintainers, end users and software evaluators |  Qualitative |  All | IC        |  The paper provides a useful basic introduction to define the different perspectives under which software quality can be analyzed |

**Quality Model** ("is based on mentions")

**NOTE: This article is mainly on context definition and its role in the process of software quality evaluation** 

The paper descrbes an extension of the ISO 9126 model os software quality, based on the findings of the project QUINT (Quality in Information Technology). 
The extension includes non-technical concepts in the software usablity ccriteria such as learnability, explicitness, clairty, helpfulness, user-friendliness. 
The results were tested by the software teams of several companies dedicated to software development, and conclusions are available in the handbook of the 
project summary. The methodology described is now embedded in the DevOps paradigms, specially concerning the need of independent testing and validation processes.

