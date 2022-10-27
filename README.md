# ili2pg-native

## todo

- Testen des fertigen native image? 


## Additional native image config files

Da noch kein GUI verwendet werden soll / unterstützt wird, muss nicht plattformabahängig die Konfig durch den Agent erstellt werden. 

```
java -agentlib:native-image-agent=config-output-dir=conf-dir -jar /Users/stefan/Downloads/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema arp_bauzonengrenzen_pub --models SO_ARP_Bauzonengrenzen_20210120 --doSchemaImport  --import /Users/stefan/Downloads/ch.so.arp.bauzonengrenzen_xtf/ch.so.arp.bauzonengrenzen.xtf
```
