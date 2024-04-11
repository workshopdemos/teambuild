# Team Build Workshop Scenario 

## Getting Started

1. Login the workshop system using the given URL, username and password
2. You are in the secure cloud environment which runs VS Code and is connected to the Mainframe
3. Make sure the initial build process has successfully completed. (**exit code: 0** message in the active terminal)
4. Close the terminal from it's right top corner

## Scenario 

**Step 1:**       
Listing the details for opening a terminal          
Select the three horizontal lines on the top left (Burger Icon) -> Terminal -> New Terminal         

Sharing a reference screenshot              
<img src='images/terminal.png' width='30%'>

**Step 2:** 

Copy paste the below command in the terminal

./exportz --environment DEV --system DOGGOS --subsystem CUST0## --sn 1 --base-url http://10.1.2.120:6002/EndevorService/api/v2  --instance ENDEVOR --user cust0## --dataset-hlq 'CUST0##.BLDZ.DOGGOS' --ssh-port 2022

**Important Notes:**          
a). Replace ## in the above command with your User ID number.       
b). The command run will prompt for a password. Enter the Password.             

Both the User ID number and Password will be shared by the instructor.          

Sharing a couple of examples of the command run:          

Example 1:       
If you are assigned User 03, then replac ## with 03 and the command will look like below:          

./exportz --environment DEV --system DOGGOS --subsystem CUST003 --sn 1 --base-url http://10.1.2.120:6002/EndevorService/api/v2  --instance ENDEVOR --user cust003 --dataset-hlq 'CUST003.BLDZ.DOGGOS' --ssh-port 2022        

Example 2:       
If you are assigned User 21, then replac ## with 21 and the command will look like below:          
  
./exportz --environment DEV --system DOGGOS --subsystem CUST021 --sn 1 --base-url http://10.1.2.120:6002/EndevorService/api/v2  --instance ENDEVOR --user cust021 --dataset-hlq 'CUST021.BLDZ.DOGGOS' --ssh-port 2022  

Sharing a couple of reference screenshots of the command run: 

<img src='images/export1.png' width='40%'>

<img src='images/export2.png' width='40%'>

**Step 3:** 

Copy paste the below command in the terminal

./syncz -a "src::bldz --proc 1"       

Sharing couple of reference screenshots of the command run: 

<img src='images/export1.png' width='40%'>

<img src='images/export2.png' width='40%'>



