# Misconfiguration Datasets
This datasets consist of real-world misconfiguration cases, papers for misconfiguration troubleshooting, and six reproduced scenarios in Docker.

- [cases/](#Misconfiguration-cases): It contains both raw data and the labeled datasets of the real-world misconfiguration cases.

- [papers/](#Misconfiguration-troubleshooting-papers): It contains a list of papers for misconfiguration troubleshooting.

- [reproduced_scenarios/](#Reproduced-misconfiguration-scenarios): It contains six reproduced real-world software misconfiguration scenarios which is wrapped Docker containers.

## Misconfiguration cases

### targets and sources
- We selected MySQL, PHP, Apache httpd, Nginx, PostgreSQL, and Hadoop as our main targets. 
- We select popular technical forums (i.e., StackOverflow and ServerFault), and official customer service channels (e.g., GitHub, Mailing lists, Offical online forums, etc.) as our data sources.

| **Software**      | **Total**  | **Auto-filtered** | **Manually filtered** |
|---------------|--------|---------------|-------------------|
| MySQL         | 25435  | 391           | 123               |
| PHP           | 41468  | 164           | 79                |
| Apache httpd  | 44146  | 510           | 187               |
| Nginx         | 24433  | 405           | 211               |
| PostgreSQL    | 7287   | 117           | 56                |
| Hadoop        | 7566   | 100           | 43                |
| Others        | 17719  | 626           | 124               |
| **Total**     | 168054 | 2313          | 823               |

### collecting and analyzing
1. We selected 2,313 solved and configuration-related cases from nearly 167.8 thousand total items.
2. we manually inspected all 2,313 cases and sampled out 823 real-world misconfigurations cases.
3. We categorized the root causes of misconfigurations into four groups, i.e., constraint violation, resource unavailability, component-dependency error, and misunderstanding of configuration effects.

| **Type**                                | **Subtype**                         | **# Cases** |
|-----------------------------------------|-------------------------------------|-------------|
| **Constraint violation**                | Syntax error                        | 52          |
|                                         | Invalid name                        | 13          |
|                                         | Misplaced configuration             | 25          |
|                                         | Duplicate option                    | 14          |
|                                         | Multi-configuration error           | 7           |
| **Resource unavailability**             | Resource identifier mismatch        | 165         |
|                                         | Resource competition                | 9           |
|                                         | Unauthorized resource access        | 58          |
|                                         | Hardware limitation                 | 8           |
| **Component-dependency error**          | Component incompatibility           | 56          |
|                                         | Component missing                   | 40          |
|                                         | Cross-component misconfiguration    | 23          |
| **Misunderstanding of configuration effects** | Business functionality deviation    | 316         |
|                                         | Performance degradation             | 20          |
|                                         | Security risk                       | 17          |


## Misconfiguration troubleshooting papers
### targets and sources
1. We conducted manual search on 13 top conferences and journals.
2. We crawled the papers from the top venues from December 2003 to September 2024. The keyword set includes `configuration\*`, `misconfiguration\*`, `configure\*`, `configuration error\*`.
and configuration fault\*.
3. We verified papers that were relevant to our research objective, i.e., software misconfiguration detection and diagnosis.
4. We searched for the papers cited by these papers or those cited these papers and identified whether they were relevant papers.

| Acronym | Venues |
|---|---|
| ASE | International Conference on Automated Software Engineering |
| ASPLOS | International Conference on Architectural Support for Programming Languages and Operating Systems |
| CCS | ACM Conference on Computer and Communications Security |
| ESEC/FSE | ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering |
| EuroSys | European Conference on Computer Systems |
| ICSE | International Conference on Software Engineering |
| NSDI | Symposium on Network System Design and Implementation |
| OOPSLA | Conference on| SOSP | ACM Symposium on Operating Systems Principles |
| TDSC | IEEE Transactions on Dependable and Secure Computing |
| TSE | IEEE Transactions on Software Engineering |
| USENIX ATC | USENIX Annual Technical Conference |

### content
The list of papers for misconfiguration troubleshooting includes `YEAR, TITLE, LINK`.

## Reproduced misconfiguration scenarios
### descriptions
Each compressed file is named after the `case ID` and only contains one real-world misconfiguration scenario.

## Cite this work
```bib
Yuhao Liu et al. "Rethinking Software Misconfigurations in the Real World: An Empirical Study and Literature Analysis"
```

