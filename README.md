# Local Mongo DB Instance

### Run: `docker-compose up`

### Done!

### Connection String

http://localhost:27017

### Expected Log:

```bash
mongodb-local-docker docker-compose up
Creating network "mongodb-local-docker_mongodb-network" with driver "bridge"
Creating volume "mongodb-local-docker-compose_dbdata" with default driver
Creating mongodb ... done
Attaching to mongodb
mongodb    | 2021-02-08T11:06:44.758+0000 I  CONTROL  [main] Automatically disabling TLS 1.0, to force-enable TLS 1.0 specify --sslDisabledProtocols 'none'
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] MongoDB starting : pid=1 port=27017 dbpath=/data/db 64-bit host=608dfbec6039
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] db version v4.2.3
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] git version: 6874650b362138df74be53d366bbefc321ea32d4
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] OpenSSL version: OpenSSL 1.1.1  11 Sep 2018
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] allocator: tcmalloc
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] modules: none
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] build environment:
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten]     distmod: ubuntu1804
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten]     distarch: x86_64
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten]     target_arch: x86_64
mongodb    | 2021-02-08T11:06:44.761+0000 I  CONTROL  [initandlisten] options: { net: { bindIp: "*" } }
mongodb    | 2021-02-08T11:06:44.761+0000 I  STORAGE  [initandlisten]
mongodb    | 2021-02-08T11:06:44.761+0000 I  STORAGE  [initandlisten] ** WARNING: Using the XFS filesystem is strongly recommended with the WiredTiger storage engine
mongodb    | 2021-02-08T11:06:44.762+0000 I  STORAGE  [initandlisten] **          See http://dochub.mongodb.org/core/prodnotes-filesystem
mongodb    | 2021-02-08T11:06:44.762+0000 I  STORAGE  [initandlisten] wiredtiger_open config: create,cache_size=482M,cache_overflow=(file_max=0M),session_max=33000,eviction=(threads_min=4,threads_max=4),config_base=false,statistics=(fast),log=(enabled=true,archive=true,path=journal,compressor=snappy),file_manager=(close_idle_time=100000,close_scan_interval=10,close_handle_minimum=250),statistics_log=(wait=0),verbose=[recovery_progress,checkpoint_progress],
mongodb    | 2021-02-08T11:06:45.214+0000 I  STORAGE  [initandlisten] WiredTiger message [1612782405:214346][1:0x7f10767adb00], txn-recover: Set global recovery timestamp: (0, 0)
mongodb    | 2021-02-08T11:06:45.221+0000 I  RECOVERY [initandlisten] WiredTiger recoveryTimestamp. Ts: Timestamp(0, 0)
mongodb    | 2021-02-08T11:06:45.231+0000 I  STORAGE  [initandlisten] Timestamp monitor starting
mongodb    | 2021-02-08T11:06:45.236+0000 I  CONTROL  [initandlisten]
mongodb    | 2021-02-08T11:06:45.236+0000 I  CONTROL  [initandlisten] ** WARNING: Access control is not enabled for the database.
mongodb    | 2021-02-08T11:06:45.236+0000 I  CONTROL  [initandlisten] **          Read and write access to data and configuration is unrestricted.
mongodb    | 2021-02-08T11:06:45.236+0000 I  CONTROL  [initandlisten]
mongodb    | 2021-02-08T11:06:45.237+0000 I  STORAGE  [initandlisten] createCollection: admin.system.version with provided UUID: 5424a1b4-9747-4e92-b349-17758bb8571e and options: { uuid: UUID("5424a1b4-9747-4e92-b349-17758bb8571e") }
mongodb    | 2021-02-08T11:06:45.248+0000 I  INDEX    [initandlisten] index build: done building index _id_ on ns admin.system.version
mongodb    | 2021-02-08T11:06:45.248+0000 I  SHARDING [initandlisten] Marking collection admin.system.version as collection version: <unsharded>
mongodb    | 2021-02-08T11:06:45.248+0000 I  COMMAND  [initandlisten] setting featureCompatibilityVersion to 4.2
mongodb    | 2021-02-08T11:06:45.248+0000 I  SHARDING [initandlisten] Marking collection local.system.replset as collection version: <unsharded>
mongodb    | 2021-02-08T11:06:45.248+0000 I  STORAGE  [initandlisten] Flow Control is enabled on this deployment.
mongodb    | 2021-02-08T11:06:45.248+0000 I  SHARDING [initandlisten] Marking collection admin.system.roles as collection version: <unsharded>
mongodb    | 2021-02-08T11:06:45.249+0000 I  STORAGE  [initandlisten] createCollection: local.startup_log with generated UUID: 54f2a54b-ee47-4dc8-b5f7-bbc836d67e9b and options: { capped: true, size: 10485760 }
mongodb    | 2021-02-08T11:06:45.258+0000 I  INDEX    [initandlisten] index build: done building index _id_ on ns local.startup_log
mongodb    | 2021-02-08T11:06:45.258+0000 I  SHARDING [initandlisten] Marking collection local.startup_log as collection version: <unsharded>
mongodb    | 2021-02-08T11:06:45.259+0000 I  FTDC     [initandlisten] Initializing full-time diagnostic data capture with directory '/data/db/diagnostic.data'
mongodb    | 2021-02-08T11:06:45.261+0000 I  SHARDING [LogicalSessionCacheRefresh] Marking collection config.system.sessions as collection version: <unsharded>
mongodb    | 2021-02-08T11:06:45.262+0000 I  CONTROL  [LogicalSessionCacheReap] Sessions collection is not set up; waiting until next sessions reap interval: config.system.sessions does not exist
mongodb    | 2021-02-08T11:06:45.262+0000 I  NETWORK  [listener] Listening on /tmp/mongodb-27017.sock
mongodb    | 2021-02-08T11:06:45.262+0000 I  NETWORK  [listener] Listening on 0.0.0.0
mongodb    | 2021-02-08T11:06:45.262+0000 I  NETWORK  [listener] waiting for connections on port 27017
mongodb    | 2021-02-08T11:06:45.262+0000 I  STORAGE  [LogicalSessionCacheRefresh] createCollection: config.system.sessions with provided UUID: a8878d3f-678a-40c5-a3a1-c315899cf676 and options: { uuid: UUID("a8878d3f-678a-40c5-a3a1-c315899cf676") }
mongodb    | 2021-02-08T11:06:45.275+0000 I  INDEX    [LogicalSessionCacheRefresh] index build: done building index _id_ on ns config.system.sessions
mongodb    | 2021-02-08T11:06:45.285+0000 I  INDEX    [LogicalSessionCacheRefresh] index build: starting on config.system.sessions properties: { v: 2, key: { lastUse: 1 }, name: "lsidTTLIndex", ns: "config.system.sessions", expireAfterSeconds: 1800 } using method: Hybrid
mongodb    | 2021-02-08T11:06:45.285+0000 I  INDEX    [LogicalSessionCacheRefresh] build may temporarily use up to 200 megabytes of RAM
mongodb    | 2021-02-08T11:06:45.285+0000 I  INDEX    [LogicalSessionCacheRefresh] index build: collection scan done. scanned 0 total records in 0 seconds
mongodb    | 2021-02-08T11:06:45.286+0000 I  INDEX    [LogicalSessionCacheRefresh] index build: inserted 0 keys from external sorter into index in 0 seconds
mongodb    | 2021-02-08T11:06:45.287+0000 I  INDEX    [LogicalSessionCacheRefresh] index build: done building index lsidTTLIndex on ns config.system.sessions
mongodb    | 2021-02-08T11:06:46.000+0000 I  SHARDING [ftdc] Marking collection local.oplog.rs as collection version: <unsharded>
mongodb    | 2021-02-08T11:06:51.998+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63164 #1 (1 connection now open)
mongodb    | 2021-02-08T11:06:52.000+0000 I  NETWORK  [conn1] received client metadata from 172.18.0.1:63164 conn1: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.4.0, LE (unified)", application: { name: "MongoDB Compass" } }
mongodb    | 2021-02-08T11:06:52.115+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63176 #2 (2 connections now open)
mongodb    | 2021-02-08T11:06:52.115+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63174 #3 (3 connections now open)
mongodb    | 2021-02-08T11:06:52.115+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63178 #4 (4 connections now open)
mongodb    | 2021-02-08T11:06:52.115+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63180 #5 (5 connections now open)
mongodb    | 2021-02-08T11:06:52.129+0000 I  NETWORK  [conn3] received client metadata from 172.18.0.1:63174 conn3: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.4.0, LE (unified)", application: { name: "MongoDB Compass" } }
mongodb    | 2021-02-08T11:06:52.130+0000 I  NETWORK  [conn2] received client metadata from 172.18.0.1:63176 conn2: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.4.0, LE (unified)", application: { name: "MongoDB Compass" } }
mongodb    | 2021-02-08T11:06:52.130+0000 I  NETWORK  [conn5] received client metadata from 172.18.0.1:63180 conn5: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.4.0, LE (unified)", application: { name: "MongoDB Compass" } }
mongodb    | 2021-02-08T11:06:52.131+0000 I  NETWORK  [conn4] received client metadata from 172.18.0.1:63178 conn4: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.4.0, LE (unified)", application: { name: "MongoDB Compass" } }
mongodb    | 2021-02-08T11:07:00.963+0000 I  NETWORK  [conn1] end connection 172.18.0.1:63164 (4 connections now open)
mongodb    | 2021-02-08T11:07:00.963+0000 I  NETWORK  [conn5] end connection 172.18.0.1:63180 (3 connections now open)
mongodb    | 2021-02-08T11:07:00.963+0000 I  NETWORK  [conn4] end connection 172.18.0.1:63178 (1 connection now open)
mongodb    | 2021-02-08T11:07:00.963+0000 I  NETWORK  [conn3] end connection 172.18.0.1:63174 (0 connections now open)
mongodb    | 2021-02-08T11:07:00.963+0000 I  NETWORK  [conn2] end connection 172.18.0.1:63176 (2 connections now open)
mongodb    | 2021-02-08T11:10:00.201+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63184 #6 (1 connection now open)
mongodb    | 2021-02-08T11:10:00.214+0000 I  NETWORK  [conn6] received client metadata from 172.18.0.1:63184 conn6: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.16.1, LE (unified)" }
mongodb    | 2021-02-08T11:10:00.293+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63188 #7 (2 connections now open)
mongodb    | 2021-02-08T11:10:00.293+0000 I  NETWORK  [conn7] received client metadata from 172.18.0.1:63188 conn7: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.16.1, LE (unified)" }
mongodb    | 2021-02-08T11:10:00.301+0000 I  SHARDING [conn7] Marking collection eeftutortool.question as collection version: <unsharded>
mongodb    | 2021-02-08T11:10:00.304+0000 I  NETWORK  [listener] connection accepted from 172.18.0.1:63192 #8 (3 connections now open)
mongodb    | 2021-02-08T11:10:00.304+0000 I  NETWORK  [conn8] received client metadata from 172.18.0.1:63192 conn8: { driver: { name: "nodejs", version: "3.6.3" }, os: { type: "Darwin", name: "darwin", architecture: "x64", version: "20.2.0" }, platform: "'Node.js v12.16.1, LE (unified)" }

```
