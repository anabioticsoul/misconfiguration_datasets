# Misconfiguration Datasets
This datasets consist of real-world misconfiguration cases, papers for misconfiguration troubleshooting, and six reproduced scenarios in Docker.

- [cases/](#Misconfiguration-cases): It contains both raw data and the labeled datasets of the real-world misconfiguration cases.

- [papers/](#Misconfiguration-troubleshooting-papers): It contains a list of papers for misconfiguration troubleshooting.

- [reproduced_scenarios/](#Reproduced-misconfiguration-scenarios): It contains six reproduced real-world software misconfiguration scenarios which is wrapped Docker containers.

## Misconfiguration cases

### Targets and sources
- We selected MySQL, PHP, Apache httpd, Nginx, PostgreSQL, and Hadoop as our main targets. 
- We select popular technical forums (i.e., StackOverflow and ServerFault), and official customer service channels (e.g., GitHub, Mailing lists, Offical online forums, etc.) as our data sources.

| **Software**      | **Total**  | **Auto-filtered** | **Manually filtered** |
|---------------|--------|---------------|-------------------|
| MySQL         | 25435  | 391           | 115               |
| PHP           | 41468  | 164           | 79                |
| Apache httpd  | 44146  | 510           | 171               |
| Nginx         | 24433  | 405           | 203               |
| PostgreSQL    | 7287   | 117           | 54                |
| Hadoop        | 7566   | 100           | 42                |
| Others        | 17719  | 626           | 108               |
| **Total**     | 168054 | 2313          | 772               |

### Collecting and analyzing
1. We selected 2,313 solved and configuration-related cases from 168,054 collected issues.
2. we manually inspected all 2,313 cases and sampled out 772 real-world misconfigurations cases.
3. We categorized the root causes of misconfigurations into four groups, i.e., constraint violation, resource unavailability, component-dependency error, and configuration semantic misinterpretation.

| **Type**                                | **Subtype**                         | **# Cases** |
|-----------------------------------------|-------------------------------------|-------------|
| **Constraint violation**                | Syntax error                        | 54          |
|                                         | Invalid name                        | 16          |
|                                         | Misplaced configuration             | 42          |
|                                         | Duplicate option                    | 21          |
|                                         | Intra-component error               | 15          |
|                                         | Cross-component error               | 23          |
| **Resource unavailability**             | Resource identifier mismatch        | 178         |
|                                         | Resource competition                | 9           |
|                                         | Unauthorized resource access        | 70          |
|                                         | Hardware limitation                 | 15          |
| **Component-dependency error**          | Component incompatibility           | 58          |
|                                         | Component missing                   | 42          |
| **Configuration semantic misinterpretation** | Ambiguous option name          | 206         |
|                             | Option value and functional requirement mismatch| 53          |


## Misconfiguration troubleshooting papers
### Targets and sources
1. We conducted manual search on 29 top conferences and journals.
2. We crawled the papers from the top venues from December 2003 to September 2024. The keyword set includes `configuration\*`, `misconfiguration\*`, `configure\*`, `configuration error\*`, and `configuration fault\*`.
3. We screened papers against our review scope and retained the studies relevant to software misconfiguration troubleshooting, (i.e., software misconfiguration detection and diagnosis).
4. We further performed backward and forward snowballing on the screened papers. Specifically, we searched for the papers cited by these papers or those cited these papers and identified whether they were relevant papers.
5. The current paper set contains 60 studies based on the revised screening results.

| **Acronym** | **Venues**                                                                                                  |
| ----------- | ----------------------------------------------------------------------------------------------------------- |
| ASE         | International Conference on Automated Software Engineering                                                  |
| ASPLOS      | International Conference on Architectural Support for Programming Languages and Operating Systems           |
| CCS         | ACM Conference on Computer and Communications Security                                                      |
| ESE         | Empirical Software Engineering                                                                              |
| ESEC/FSE    | ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering |
| EuroSys     | European Conference on Computer Systems                                                                     |
| ICPC        | IEEE International Conference on Program Comprehension                                                      |
| ICSE        | International Conference on Software Engineering                                                            |
| IETS        | IET Software                                                                                                |
| IST         | Information and Software Technology                                                                         |
| ISSTA       | International Symposium on Software Testing and Analysis                                                    |
| JFP         | Journal of Functional Programming                                                                           |
| JSS         | Journal of Systems and Software                                                                             |
| NSDI        | Symposium on Network System Design and Implementation                                                       |
| OOPSLA      | Conference on Object-Oriented Programming Systems, Languages, and Applications                              |
| OSDI        | USENIX Symposium on Operating Systems Design and Implementation                                             |
| RE          | Requirements Engineering                                                                                    |
| SCP         | Science of Computer Programming                                                                             |
| SOSP        | ACM Symposium on Operating Systems Principles                                                               |
| SoSyM       | Software and Systems Modeling                                                                               |
| SPE         | Software: Practice and Experience                                                                           |
| SPLC        | International Systems and Software Product Line Conference                                                  |
| STVR        | Software Testing, Verification and Reliability                                                              |
| TDSC        | IEEE Transactions on Dependable and Secure Computing                                                        |
| TOPLAS      | ACM Transactions on Programming Languages and Systems                                                       |
| TOSEM       | ACM Transactions on Software Engineering and Methodology                                                    |
| TSC         | IEEE Transactions on Services Computing                                                                     |
| TSE         | IEEE Transactions on Software Engineering                                                                   |
| USENIX ATC  | USENIX Annual Technical Conference                                                                          |


### Content
The list of papers for misconfiguration troubleshooting includes `Year`, `Info`, and `Link`.

## Reproduced misconfiguration scenarios
### Description
Each compressed file is named after the `case ID` and only contains one real-world misconfiguration scenario.

## Cite this work
We would appreciate it if you cite this paper utilizing the misconfiguration datasets in your research work: Yuhao Liu et al. "Rethinking Software Misconfigurations in the Real World: An Empirical Study and Literature Analysis".
```bib
@article{liu2024rethinking,
  title={Rethinking Software Misconfigurations in the Real World: An Empirical Study and Literature Analysis},
  author={Liu, Yuhao and Zhou, Yingnan and Zhang, Hanfeng and Chang, Zhiwei and Xu, Sihan and Jia, Yan and Wang, Wei and Liu, Zheli},
  journal={arXiv preprint arXiv:2412.11121},
  year={2024}
}
```
