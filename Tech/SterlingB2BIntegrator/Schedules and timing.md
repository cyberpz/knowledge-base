```sql 
--- Find Schedules Service name and timing #Sterling
SELECT SERVICENAME,
utl_raw.cast_to_varchar2(dbms_lob.substr( utl_compress.lz_uncompress(dt.DATA_OBJECT)) ) TimingXML
FROM SCHEDULE s
JOIN DATA_TABLE dt ON dt.DATA_ID = TIMINGXML
WHERE status = 'ACTIVE' AND dt.REFERENCE_TABLE = 'SCHEDULE' AND ROWNUM <= 100
ORDER BY SERVICENAME;
```

> [!note] Still needs to parse and beautify the XML from TimingXML.

Preview:
![[Pasted image 20230210161713.png]]