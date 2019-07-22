## FIREBIRD

##### Check for errors
```
gfix -v -full C:\path\database.fdb -user SYSDBA -pass masterkey
```

##### Try to fix errors
```
gfix -mend -full -ignore C:\path\database.fdb -user SYSDBA -pass masterkey
 ```
##### Create backup
```
gbak -b -user SYSDBA -password masterkey c:\path\database.fdb c:\path\database.gbk
```

##### Restore backup
```
gbak -r -user SYSDBA -password masterkey c:\path\database.gbk c:\path\database_restored.fdb
```

##### SOURCE: Adapted from http://delphiparainiciantes.com.br/diagnosticando-e-recuperando-banco-de-dados-firebird-corrompido/
