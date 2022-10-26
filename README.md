# ili2pg-native


```
java -agentlib:native-image-agent=config-output-dir=conf-dir-osx -jar /Users/stefan/Downloads/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema foo1 --models SO_ARP_Bauzonengrenzen_20210120  --schemaimport

java -agentlib:native-image-agent=config-output-dir=conf-dir-osx -jar /Users/stefan/Downloads/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema foo1 --models SO_ARP_Bauzonengrenzen_20210120  --import /Users/stefan/Downloads/ch.so.arp.bauzonengrenzen_xtf/ch.so.arp.bauzonengrenzen.xtf


java -agentlib:native-image-agent=config-output-dir=conf-dir-osx -jar /Users/stefan/Downloads/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema foo1 --models SO_ARP_Bauzonengrenzen_20210120  --export fubar.xtf
```

```
java -agentlib:native-image-agent=config-output-dir=conf-dir-osx -jar /Users/stefan/Downloads/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema foo1 --models SO_ARP_Bauzonengrenzen_20210120 --doSchemaImport  --import /Users/stefan/Downloads/ch.so.arp.bauzonengrenzen_xtf/ch.so.arp.bauzonengrenzen.xtf
```

```
./build/native/nativeCompile/ili2pg --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema foo2 --models SO_ARP_Bauzonengrenzen_20210120 --doSchemaImport  --import /Users/stefan/Downloads/ch.so.arp.bauzonengrenzen_xtf/ch.so.arp.bauzonengrenzen.xtf


```