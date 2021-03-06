# Pentester-Red-Team-vs.-SOC-Analyst-Blue-Team-
In this project, as the Red Team, I pentested a vulnerable VM within a virtual environment, ultimately gaining root access to the machine. As Blue Team, I used Kibana to review logs taken during the pentesting engagement. I used the logs to extract hard data and visualizations for a report.

## Red Team
* Discover the IP address of the Linux web server.

![image](https://user-images.githubusercontent.com/87041507/147603388-401d7b51-ed1d-4391-a43a-ce629bd6796a.png)

* Locate the hidden directory on the web server.

![image](https://user-images.githubusercontent.com/87041507/147603439-dbbd7ebe-6bde-42e8-ab90-11431c5caae6.png)
![image](https://user-images.githubusercontent.com/87041507/147603460-3de3eff8-d0f8-417d-b571-9d8b4f791549.png)

* Brute force the password for the hidden directory using the hydra command

![image](https://user-images.githubusercontent.com/87041507/147603481-3d293a5a-9e6d-4a1f-b7ad-69e647e42111.png)
![image](https://user-images.githubusercontent.com/87041507/147603506-eacb2de7-7038-46f0-8af9-d44d498b4f63.png)
![image](https://user-images.githubusercontent.com/87041507/147603527-56193a5b-5ea1-4a5e-b6e6-b3d463c6357f.png)

* Break the hashed password with the Crack Station website or John the Ripper.

![image](https://user-images.githubusercontent.com/87041507/147603546-d590682c-6356-4b43-a81b-59d609679a8b.png)

* Connect to the server via WebDav.

![image](https://user-images.githubusercontent.com/87041507/147603573-0fcdac7c-eeeb-4fac-963a-bdac45837cd0.png)

* Upload a PHP reverse shell payload.

![image](https://user-images.githubusercontent.com/87041507/147603596-f8ffd455-69d8-4e2e-be82-1a9573538e86.png)
![image](https://user-images.githubusercontent.com/87041507/147603639-88c254e5-25de-4983-a4d7-470d0e3ae82e.png)
![image](https://user-images.githubusercontent.com/87041507/147603655-59eb9874-5ba0-4d55-a087-42e0a13e106a.png)

* Execute payload that you uploaded to the site to open up a meterpreter session.

![image](https://user-images.githubusercontent.com/87041507/147603688-70348149-185e-4543-bd4c-8b869bfb871c.png)
![image](https://user-images.githubusercontent.com/87041507/147603704-caf7548b-8250-49f7-9a01-83d53d251538.png)
![image](https://user-images.githubusercontent.com/87041507/147603722-bc30aa11-75e1-4fb0-9109-16b663dd6fdb.png)
![image](https://user-images.githubusercontent.com/87041507/147603746-a9d99404-87a3-48f7-bcb9-cdc6dd1cc51f.png)

* Find and capture the flag.

![image](https://user-images.githubusercontent.com/87041507/147603778-23bc5807-76ef-4d61-bf35-538d7b4c446c.png)
![image](https://user-images.githubusercontent.com/87041507/147603794-ce706b21-acf1-48df-82c8-3a321d3b846a.png)
![image](https://user-images.githubusercontent.com/87041507/147603819-7f1b03c3-8c45-4616-98d1-01e3d85b4ab0.png)
![image](https://user-images.githubusercontent.com/87041507/147603831-574b03e8-d2da-49a0-acca-b697d53fa39d.png)

## Blue Team
* Identify the offensive traffic.

![image](https://user-images.githubusercontent.com/87041507/147604017-e7cfe3d6-5204-48de-a923-632b86704580.png)
![image](https://user-images.githubusercontent.com/87041507/147604043-ec2fd604-db46-4ab6-bc77-219a6ac77b11.png)
![image](https://user-images.githubusercontent.com/87041507/147604061-5e171b6b-26a8-44d1-bec1-eba20dd395a3.png)

* Find the request for the hidden directory.

![image](https://user-images.githubusercontent.com/87041507/147604098-cdfc90bb-830b-4de8-a3e5-49fd981df2ee.png)
![image](https://user-images.githubusercontent.com/87041507/147604112-ff980467-9d2c-4a25-bf1f-284a79bfaa84.png)

* Identify the brute force attack.

![image](https://user-images.githubusercontent.com/87041507/147604135-6c149cc7-4beb-4a99-81f1-de92d81d338d.png)
![image](https://user-images.githubusercontent.com/87041507/147604156-fe8e0fd0-f703-435f-87e7-1ae1d4486e78.png)

* Find the WebDav connection.

![image](https://user-images.githubusercontent.com/87041507/147604217-bd628496-9b60-4170-88ad-5bb84ef2e143.png)

* Identify the reverse shell and meterpreter traffic.

![image](https://user-images.githubusercontent.com/87041507/147604240-11c32463-5089-4b7d-bc1b-52d2452c641d.png)




