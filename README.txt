wower

wower is Erlang implementation of World of Warcraft server emulator.

== Current status ==

Working with WoTLK 3.0.8.

=== Logon server ===

Allows you to connect and select realm.
Does not support reconnect after wrong password.
Does not support patching.

=== Realm server ===

Accepts connections. Packet encryption/decryption implemented.
Character list implemented. Login into world implemented.
You can now run around with default character with some strange
absolutely random display id.

Creating character works. Importing DBC files works. Cell system 
works.

=== Get started ===

1. Install Erlang (http://erlang.org/download.html)
2. Install Git (for Windows http://code.google.com/p/msysgit/, for Ubuntu Desktop sudo apt-get install git-core)
3. Get sources via Git (git clone git://github.com/SneakerXZ/wower.git) 
4. Go to directory with wower source
5. Make a directory ebin
6. Run `erl -make` 
7. Go to ebin folder
8. Run `erl` and type next commands:
   > helper:install(). // only if you want to recreate DB
   > helper:start().   // this will start realm and logon serversd logon servers

You must have correct(>= 3.0.8) DBC files in ebin/dbc folder to
start server properly.

=== Working on ===

Moving packets.
