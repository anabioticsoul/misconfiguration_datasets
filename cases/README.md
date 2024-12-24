# Misconfiguration cases
### Raw dataset
It is a raw dataset without labels, including `Software`, `Link`, `Description`, `Year`, and `Last Modified`. 
- `Year`: The time when the user raised the issue of configuration errors.
- `Last Modified`: The last time this issue was modified.

### Labeled dataset
It is a dataset labeled with root causes, including `ID`,`Software`, `Link`, `Description`, `Subtype`, `Year`, and `Last Modified`. 
- `ID`: CA, CB, CC, and CD are used to denote the cases whose root causes are constraint violation, environment error, component-dependency error, and misunderstanding of configuration effects.
- `Subtype`: The subtypes of each root causes. E.g., the subtypes of constraint violation are syntax error, invalid option name, misplaced configuration, duplicate option, and multi-configuration error.
