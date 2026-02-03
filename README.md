# Efemeral
Single-file IRC-style P2P CLI chat.
IP-based, no encryption.
Made on Linux Mint. Probably won’t work on Windows.

I know it's bad. It was made by a beginner. what do you expect?

v0.1.2 is the latest version. Anything before latest version is likely to have bugs.

Usage: 

To open an instance: ``efemeral_cli --host <0.0.0.0> --port <PORT> --passphrase <PASSPHRASE>`` and optionally ``--nick <NICK>``. If you do not specify a nickname, it will default to your endpoint. 

<img width="657" height="415" alt="image" src="https://github.com/user-attachments/assets/f51a89d7-c90f-4ef1-88d7-02c965ba6d25" />


You can change your nick at any time with ?nick.
For most users, 0.0.0.0 is what you'll use for host. it'll accept connections from any source. Port is whatever port you want the server to open to. 
When you open an instance, you'll be given a link. The link will look something like ``efemeral://<host>:<port>/<passphrase>`` and is needed for anybody to join your instance. Anybody you want to join will also need the port you used to launch the instance in order to connect. Since this is encoded in the link, i'll add a feature to automate this in the future, but for now you'll need to tell them this, too.

<img width="649" height="248" alt="image" src="https://github.com/user-attachments/assets/6c040eab-b71f-44d2-bbe2-a4b4cfd58ec6" />


When in an instance as the host, you can ?kick users. ?ban also works, but currently there's no distinction. ``?kick <nick>``

<img width="355" height="153" alt="image" src="https://github.com/user-attachments/assets/c00d3ed9-b479-4e69-8598-61b2f235094c" />


To close the instance, close the command line, or interrupt with ctrl C.

You can use ?color <hex> to change the color of your nick. 

To join an instance, you need the instance link, and the port. The host should tell you what port they're using. Run ``efemeral_cli --link <LINK> --port <PORT>`` and optionally ``--nick <NICK>``. If you do not specify a nickname, it will default to your endpoint. You can change your nick at any time with ?nick.



CC-BY-SA 4.0
See LICENSE for more details.

The comment in efemeral_cli.py is a joke; disregard it. 


<img width="485" height="712" alt="image" src="https://github.com/user-attachments/assets/5e65be05-8617-44c7-bc57-07d112de0d89" />
