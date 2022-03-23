# PocketMonstersOnline

## Server

set up MySQL, then `$ mysql -uroot -prootpassword < Server/pokenetdb_blank.sql`

```
$ cd Server
$ javac -cp .:./lib/* src/**/*.java && java --add-opens java.base/java.lang=ALL-UNNAMED -cp lib/*:src org.pokenet.server.GameServer -s low
```

## Client

```
$ cd Client
$ javac -cp .:./lib/* src/**/*.java && java -cp lib/*:src -Djava.library.path=lib/native org.pokenet.client.GameClient
```

(haven't figured out how to recompile yet)
