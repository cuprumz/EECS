### garbage collection







`Eden Space`

`Survivor#0` `Survivor#1` : S0 = S1

`Old Space`

`Metaspace`

`Perm Space`



`Young Generation`: *Eden Space* + *Survivor#0* + *Survivor#1*

`Tenured Generation`:  *Old Space* + *Metaspace*/*Perm Space*

`Metaspace`/`Perm Space`: 

- \< *JDK1.8* *Permanent Generation*
- \>*JDK1.8* *Metaspace*: constant, method meta data, class meta data



`XX:MaxMetaspaceSize=256M -Xms4g -Xmx4g -Xmn1g -Xss256k -XX:SurvivorRatio=8  -XX:MaxTenuringThreshold=8, -XX:ParallelGCThreads=8, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+DisableExplicitGC, -XX:+CMSParallelRemarkEnabled, -XX:+CMSClassUnloadingEnabled, -XX:CMSInitiatingOccupancyFraction=70, -XX:CMSFullGCsBeforeCompaction=5, -XX:+UseCMSCompactAtFullCollection, -XX:+CMSScavengeBeforeRemark, -XX:+HeapDumpOnOutOfMemoryError, -Xloggc:/usr/local/webserver/voice-analyzer-web/logs/gc.log, -XX:+UseGCLogFileRotation, -XX:NumberOfGCLogFiles=10, -XX:GCLogFileSize=10M, -XX:+PrintGCDetails, -XX:+PrintGCDateStamps, -XX:+PrintGCApplicationStoppedTime, -XX:+PrintGCApplicationConcurrentTime, -, -XX:HeapDumpPath=/usr/local/webserver/voice-analyzer-web/logs/voice-analyzer-web.hprof `



`-Xms`: initial *heap* size

`-Xmx`: maximum *heap* size

`-Xss`: *VM* stack size

`-Xmn` *Young Generation* size. initial and max.

`-XX:SurvivorRatio`: *Eden*/*Survivor#0*. default 8, means Eden:S0:S1=*8:1:1*

`-XX:NewRatio`: *Tenured Generation*/*Young Generation*. default 2, means TenuredGen:YoungGen=2:1

`-XX:MetaspaceSize`: initial *Metaspace* size

`-XX:MaxMetaspaceSize`: max *Metaspace* size

`-XX:PermSize`: initial permanent size

`-XX:MaxPermSize`: max permanent size





: *Young Generation*. called *Minor GC*

 called *Full GC*

