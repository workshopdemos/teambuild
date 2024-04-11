# Team Build Workshop Scenario 

## Getting Started

1. Login the workshop system using the given URL, username and password
2. You are in the secure cloud environment which runs VS Code and is connected to the Mainframe
3. Make sure the initial build process has successfully completed. (**exit code: 0** message in the active terminal)
4. Close the terminal from it's right top corner

## Scenario 

Step 1: Open the Command line Terminal.
Select the three vertical lines on the top left (Burger Icon) -> Terminal -> New Terminal. 
Sharing a reference screenshot

<img src='images/terminal.png' width='30%'>

Step 2: 

Copy paste the below command in the command line terminal

./exportz --environment DEV --system DOGGOS --subsystem CUST0## --sn 1 --base-url http://10.1.2.120:6002/EndevorService/api/v2  --instance ENDEVOR --user cust0## --dataset-hlq 'CUST0##.BLDZ.DOGGOS' --ssh-port 2022

Replace ## in the above command with your User ID number. Sharing couple of examples: 

If you are assinged User 21, then the command will be: 

./exportz --environment DEV --system DOGGOS --subsystem CUST021 --sn 1 --base-url http://10.1.2.120:6002/EndevorService/api/v2  --instance ENDEVOR --user cust021 --dataset-hlq 'CUST021.BLDZ.DOGGOS' --ssh-port 2022


If you are assinged User 03, then the command will be: 

./exportz --environment DEV --system DOGGOS --subsystem CUST003 --sn 1 --base-url http://10.1.2.120:6002/EndevorService/api/v2  --instance ENDEVOR --user cust003 --dataset-hlq 'CUST003.BLDZ.DOGGOS' --ssh-port 2022


Step 3: 

Copy paste the below comand in the command line terminal

./syncz -a "src::bldz --proc 1"


