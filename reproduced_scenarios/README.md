# Reproduced cases
### Description
- `CA14`: The `default-time-zone` option in the my.cnf file is incorrectly set with underscores instead of dashes.
- `CA35`: The `password` option is missing the quotes around the option value.
- `CA54`: The tag `<configuration>...</configuration>` is written twice in four XML files.
- `CB116`: The `bind-address` option is set incorrectly to an invalid IP address by default.
- `CD202`: The `fs.defaultFS` option is set to a wrong path.
- `CD223`: The `log_queries_not_using_indexes` option is set to `on` by default.

### Usage
1. Download the compressed files of reproduced scenarios.
2. Import the docker image from the compressed files.
```sh
docker import [CaseID].tar.gz [image-name]:latest
```
3. Run scenarios
```sh
docker run -it [image-name] bash
```
