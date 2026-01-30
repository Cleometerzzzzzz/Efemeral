# Efemeral
An IRC-style peer-to-peer Command Line Chat that's lightweight and heavily customizable.
Uses IP for now; i couldn't figure out how to implement I2p. It's not end-to-end encrypted, so be warned.

I know it's bad. It was made by a beginner. what do you expect?

Usage: 

To open an instance: ``efemeral_cli --host <0.0.0.0> --port <PORT> --passphrase <PASSPHRASE>`` and optionally ``--nick <NICK>``. If you do not specify a nickname, it will default to your endpoint. You can change your nick at any time with ?nick.
For most users, 0.0.0.0 is what you'll use for host. it'll accept connections from any source. Port is whatever port you want the server to open to. 
When you open an instance, you'll be given a link. The link will look something like ``efemeral://<host>:<port>/<passphrase>`` and is needed for anybody to join your instance.
When in an instance as the host, you can ?kick users. ?ban also works, but currently there's no distinction. ``?kick <nick>``
To close the instance, close the command line.


To join an instance, you need the instance link. Run ``efemeral_cli --link <link>`` and optionally ``--nick <NICK>``. If you do not specify a nickname, it will default to your endpoint. You can change your nick at any time with ?nick.
