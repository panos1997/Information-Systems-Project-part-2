# InformationSystemsProject_2 written in C

## Given batches of queries as input find the row ids of the tables that satisfy the predicates.
### A predicate can be of 2 types, either a filter or a join. An exampe of an input could be "0 2 4|0.1=1.2&1.0=2.1&0.1>3000|0.0 1.1" which is translated to SQL like this: 
#### SELECT SUM("0".c0), SUM("1".c1) 
#### FROM r0 "0", r2 "1", r4 "2"
#### WHERE 0.c1=1.c2 and 1.c0=2.c1 and 0.c1>3000

