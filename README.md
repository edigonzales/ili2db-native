# ili2pg-native

Native Images von _ili2pg_ für Windows, macOS und Linux. Java wird nicht mehr benötigt. Die grafische Oberfläche wird nicht unterstützt.

```
./ili2pg --help
```

Für jede Version von _ili2pg_ gibt es einen Branch, z.B. `V_4_9_1`. Das Native Image wird als Zip-Datei unter https://github.com/edigonzales/ili2pg-native/releases veröffentlicht. Die Zahl nach dem Unterstrich entspricht der Buildnummer der Github-Action. Der main-Branch kann keine Releases machen.


## Develop

Da noch kein GUI verwendet werden soll / unterstützt wird, müssen die GraalVM-Konfig-Dateien durch den Agent nicht plattformabahängig erstellt werden. 

Beispiel-Aufruf mit einem einfachen XTF:
```
java -agentlib:native-image-agent=config-output-dir=conf-dir -jar /Users/stefan/Downloads/ili2pg-4.9.0/ili2pg-4.9.0.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr ddluser --dbpwd ddluser --nameByTopic --defaultSrsCode 2056 --strokeArcs --dbschema arp_bauzonengrenzen_pub --models SO_ARP_Bauzonengrenzen_20210120 --doSchemaImport  --import /Users/stefan/Downloads/ch.so.arp.bauzonengrenzen_xtf/ch.so.arp.bauzonengrenzen.xtf
```
