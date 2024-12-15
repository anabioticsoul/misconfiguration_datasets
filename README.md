# Misconfiguration Datasets
This datasets consist of real-world misconfiguration cases, papers for misconfiguration troubleshooting, and six reproduced scenarios in Docker.
cases/: It contains both raw data and the labeled datasets of the real-world misconfiguration cases.
papers/: It contains a list of papers for misconfiguration troubleshooting.
reproduced_scenarios/: It contains six reproduced real-world software misconfiguration scenarios which is wrapped Docker containers.

## Misconfiguration cases

### targets and sources
- We selected MySQL, PHP, Apache httpd, Nginx, PostgreSQL, and Hadoop as our main targets. 
- We select popular technical forums (i.e., StackOverflow and ServerFault), and official customer service channels (e.g., GitHub, Mailing lists, Offical online forums, etc.) as our data sources.

| Software      | Total  | Auto-filtered | Manually filtered |
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



## Misconfiguration troubleshooting papers
TODO

## Reproduced misconfiguration scenarios
TODO
