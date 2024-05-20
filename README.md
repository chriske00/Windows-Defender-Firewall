# Windows Defender Firewall


## Objective
•Configure Firewall Rules Using Windows Defender Firewall

•Configure Firewall Rules Using Windows Defender Firewall with Advanced Security

### Skills Learned

• Understanding Windows Defender Firewall

• Configuring Firewall Rules Using Windows Defender Firewall

• Configuring Firewall Rules Using Windows Defender Firewall with Advanced Security

• Editing Existing Firewall Rules

• Creating Custom Firewall Rules

## Steps
1) Click the Windows Start button. Then select Windows Security and click Firewall & network protection to see firewall status :


 
 <img width="588" alt="2,1" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/742078ba-5f76-4251-97c7-e13a7a658190">


 
 2) Click on each network to verify that the Windows Defender Firewall is toggled to on



<img width="498" alt="1,3" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/1b4a4d9e-7cca-4cef-9e9a-e652c8cfbcc8">


See the option Incoming connections. If you need to block all incoming domain network traffic, including traffic that is typically allowed, then you only need to activate this option.




3) Select the back arrow button to return to the Firewall and network protection window. Click Allow an app through firewall. Scroll to google Chrome OR Mozilla Firefox. Observe in the screenshot below that the current configuration allows for Firefox to communicate on the Private network only but denies it from communicating on the Public network.




<img width="542" alt="1,5" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/e98c90f5-a50d-467b-8be6-1e957bb20a52">


4) Select Advanced settings on the Firewall & network protection screen.


<img width="588" alt="2,1" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/99367264-8f02-451c-8925-322ded63f554">


5) Here you will see an Overview in the center panel. Make special note of the two rule types listed on the left panel:

Inbound rules: Inbound rules determine what traffic is allowed to the computer.
Outbound rules: Outbound rules determine what traffic is allowed to leave the computer.
Connection security rules
Monitoring

<img width="572" alt="Screenshot 2024-05-20 alle 17 42 46" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/e38be1ca-36d4-4229-a203-acb96f1b0b74">


6) Scroll to the Key Management Service inbound rule in the Overview panel of Windows Defender Firewall with Advanced Security. Note the following:
The policy is currently not enabled (the Enabled column says No.)

<img width="820" alt="Screenshot 2024-05-20 alle 17 39 26" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/cac311d7-a392-4d36-bc77-00c57645581d">


7) Click the Advanced tab. Here you will see which profiles the rule applies to. In this case, Domain, Private and Public are all selected. Because we want to allow communication only with the domain and private networks, For Public this box should not have a checkmark. 

<img width="807" alt="Screenshot 2024-05-20 alle 17 52 49" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/5a35f42a-d92b-4421-8677-6b8ce721d64e">


8) Now we will create an inbound rule that blocks communication with the public network. Since the new rule will be similar to the last, we will copy the existing rule. Right-click the Key Management Service (TCP-In) in bound rule and click by pressing copy and pressing Ctrl+V to paste.

  
11) <img width="642" alt="Screenshot 2024-05-20 alle 17 57 03" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/3f4621ca-b619-4b7b-9d43-86cfef05da6b">


12) Since we want to block connection with the public network, select Block the connection on the General tab. Click Apply. Then from Advanced tab the Domain and Private boxes to remove the checkmarks.

<img width="808" alt="Screenshot 2024-05-20 alle 18 02 02" src="https://github.com/chriske00/Windows-Defender-Firewall/assets/170177508/3da2f5f8-f46f-481e-be2a-7b7e52750e8d">

    
