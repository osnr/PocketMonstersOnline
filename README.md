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
$ java -Djava.library.path=lib/native -jar Pokenet.jar
```

(haven't figured out how to recompile yet)
