
DevOps – Security and Compliance CST 8919
Catherine Daigle - 41175118

# Lab Assignment: Grafana Installation and Dashboard Creation for Ubuntu Server Performance

## Objective:
Install Grafana onto an Ubuntu machine, set up Azure Monitor and create a Grafana Dashboard

## Screenshots:

### Task 1: Prepare Your Ubuntu Server
Creating VM
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.47.12 PM.png>)

Connecting to VM Via SSH:
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.50.08 PM.png>)

Terminal connection:
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.52.43 PM.png>)

Prepare server
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.53.06 PM.png>)

### Task 2: Install Grafana
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.54.53 PM.png>)
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.55.34 PM.png>)

Starting Grafana:
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.56.42 PM.png>)

### Task 3: Enable Port 3000	
![alt text](<Screenshots/Screenshot 2025-03-19 at 4.57.44 PM.png>)

### Task 4: Set Roles
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.01.43 PM.png>)
I added role assignments on both VM level and subscription level just In case.

![alt text](<Screenshots/Screenshot 2025-03-19 at 5.19.08 PM.png>)
I also created a log analytics workspace/data collection rule and followed Lab 2, but I am not sure If that was needed.

### One of the common errors was a authentication error, Authentication had to be switched to Entra ID:
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.26.00 PM.png>)
Setting managed identity = true for Grafana authentication method
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.42.20 PM.png>)


### Task 5: Log into Grafana Add Azure as a Data source:
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.00.07 PM.png>)
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.44.36 PM.png>)

### Task 6: Create Dashboard:
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.55.06 PM.png>)
Selecting data source & resource as the VM
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.55.11 PM.png>)
![alt text](<Screenshots/Screenshot 2025-03-19 at 5.58.25 PM.png>)

Below you set Resources as the VM and pick the metrics in this case it is networks, The form of the graph is edited as the pie chart section to the right.
![alt text](<Screenshots/Screenshot 2025-03-19 at 6.36.55 PM.png>)

Wanted to create a CPU usage Dial
![alt text](<Screenshots/Screenshot 2025-03-19 at 6.38.29 PM.png>)

## Finished Dashboard:
This is the dashboard within 1 hour of monitoring VM
![alt text](<Screenshots/Screenshot 2025-03-19 at 6.44.35 PM.png>)

This is Dashboard within 30 min of Monitoring.
![alt text](<Screenshots/Screenshot 2025-03-19 at 6.44.42 PM.png>)
