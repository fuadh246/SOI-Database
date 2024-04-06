# SOI-Database
CIS 4331 Final project


# Project tree

.
 * [Data](./Data)
   * [BCRED_soi_tables.xlsx](./Data/BCRED_soi_tables.xlsx)
 * [README.md](./README.md)
 * [ERD](./ERD)
   * [ERD.png](./ERD/ERD.png)
   * [ERD.drawio](./ERD/ERD.drawio)
   * [Schema.drawio](./ERD/Schema.drawio)
   * [Schema.png](./ERD/Schema.png)
 * [Docs](./Docs)
   * [Part 1 Deliverable.pdf](./Docs/Part 1 Deliverable.pdf)
 * [SQL](./SQL)


### run this to get the tree
```bash
#run this to get the tree
#!/bin/bash
#File: tree-md

tree=$(tree -tf --noreport -I '*~' --charset ascii $1 |
       sed -e 's/| \+/  /g' -e 's/[|`]-\+/ */g' -e 's:\(* \)\(\(.*/\)\([^/]\+\)\):\1[\4](\2):g')

printf "# Project tree\n\n${tree}"
```