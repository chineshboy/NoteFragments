#### python3：(unicode error) 'utf-8' codec can't decode
Error: SyntaxError: (unicode error) 'utf-8' codec can't decode byte 0xb4 in position 0:invalid start byte.

Possible reason: python file is not stored in utf-8 encoding.

Solution: convert the python file into utf-8 encoding.

#### mysql cannot start due to disk-full, broken files or other reasons
Solution: in my.cnf, set "innodb_force_recovery" from 1 to 6. The higher number, the less function, but more likely to ignore some errors. ***High number may prevent data recovery!***
