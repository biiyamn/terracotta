# Project Title
Terracotta jvm clustering labs
# Getting Started
### Prerequisites
* Download terracotta 3.7.10
 ``` wget http://d2zwv9pap9ylyd.cloudfront.net/terracotta-3.7.10.tar.gz ```
* Download java 6 (dso is incompatible with java 7 & 8 but terracotta server is compatible with java 8)
```https://confluence.terracotta.org/display/release/Terracotta+3.7```
* DSO features will no longer be included in Terracotta products from v4 use big memory instead
```https://confluence.terracotta.org/pages/viewpage.action?pageId=37129634#ChangestoOpen-SourceTerracottaServerArrayandTerracottaDSO(FAQ)-What'shappeningwithTerracottaDSO?```
* for previous release ```https://confluence.terracotta.org/display/release/BigMemory+Release+Archive```
# lab1 counter
* mvn compile
* export JAVA_HOME=~/Downloads/jdk1.6.0_45/
* start terracotta server:  terracotta-3.7.10/bin/start-tc-server.sh
* cd counter/target/classes
* console1 : terracotta-3.7.10/platform/bin/dso-java.sh -cp . tc/Counter
* console2 : terracotta-3.7.10/platform/bin/dso-java.sh -cp . tc/Counter
#Technical tips
## On-heeap off-heap
* https://stackoverflow.com/questions/6091615/difference-between-on-heap-and-off-heap
* https://code.google.com/archive/p/fast-serialization/wikis/QuickStartHeapOff.wiki
## bigmemory
* https://stackoverflow.com/questions/39578358/differences-between-ehcache-3-offheap-storage-and-bigmemory






