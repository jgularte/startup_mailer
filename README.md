# startup_mailer
Use this file to have your raspberry pi email its IP Address to you

## Step One: Create Gmail Account
  1. You will need a gmail account to act as a sender. Create a free gmail account and remember the 
      email and password.

## Step Two: Create directory and file
  1. mkdir Code && cd Code
  2. sudo nano startup_mailer.py
  3. enter the email you want to send to as well as the email and pasword your created
  
 ## Step Thee: Add file to the boot up routine
  1. cd /etc
  2. sudo nano rc.local
  3. add this line under the print cammand in the if statement: 
       "python /home/pi/Code/startup_mailer.py"
  4. Save and reboot
