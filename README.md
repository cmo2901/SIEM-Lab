# SIEM Implementation with Microsoft Azure

## Objective
In this project, I deployed a virtual machine with weak credentials and port 3389 open to the external web. I created event rules that would send an alert when detecting successful logins to the virtual machine.

### Tools Used
<p> Microsoft Azure <br>
Microsoft Sentinel </p>

### Skills Learned
<p> Log Analysis <br>
Threat Detection </p>


### Configuration of Workspace & Virtual Machine
<p> Virtual Machine with port 3389 open and weak credentials:</p>

![SIEM Step 2](https://github.com/user-attachments/assets/07670910-518a-44fa-aecc-35836eac5d2e)



<p> Workspace for log analysis:</p>

![SIEM Step 3](https://github.com/user-attachments/assets/1a60425f-ea7b-495b-9264-5b641ee3e04e)


### Alert Rule for Successful Login Attempts

![SIEM Step 5a](https://github.com/user-attachments/assets/c9498c02-2811-4f9e-a7d2-8466d92184d5)

![SIEM Step 5b](https://github.com/user-attachments/assets/a398731e-9489-4f08-b853-5b9b3b0fa9bf)

<p> This query will run automatically every 5 minutes, searching the logs for successful login attempts on the virtual machine. <br>
By setting an alert threshold of greater than zero, an alert will generate on the first successful login:</p>

![SIEM Step 5c](https://github.com/user-attachments/assets/a20f2469-5216-4aab-acdd-c8b49ed8e6c9)

<p> From here, I can monitor events relating to my virtual machine for alerts:</p>

![SIEM events](https://github.com/user-attachments/assets/053e244c-795c-43d7-b654-055b5623a549)




