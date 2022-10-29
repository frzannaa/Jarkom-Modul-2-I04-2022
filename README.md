# Jarkom-Modul-2-I06-2022
<strong> Our Members :
1. Farzana Afifah Razzak - 5025201130
2. 
3. </strong>

## 1. All nodes are connected to Ostania as the router, so they can access the internet. so we ping all node
![image](https://user-images.githubusercontent.com/81352414/198834631-a66567ca-218b-43c9-b2c6-267e94d9dc18.png)
![image](https://user-images.githubusercontent.com/81352414/198834652-23b6ae63-1de1-4455-a85d-525cc5180431.png)
![image](https://user-images.githubusercontent.com/81352414/198834696-a20fac31-c0c6-40c1-9f68-50a62f2bc231.png)
![image](https://user-images.githubusercontent.com/81352414/198834707-2dff4e23-5fd7-4649-9706-2befc60722ec.png)
![image](https://user-images.githubusercontent.com/81352414/198834730-89623cfe-8357-4d51-8354-ae6c60e54949.png)
![image](https://user-images.githubusercontent.com/81352414/198834749-74ce500f-2411-4d84-bcc5-b7271dd0f90a.png)

## 2. Help Loid create the main website by accessing wise.yyy.com with alias www.wise.yyy.com on the wise folder

first make dns as usual

![image](https://user-images.githubusercontent.com/81352414/198834940-76ffa5db-0a04-4bd2-9f4b-8d83f687a5e0.png)

then we open `/etc/bind/wise/wise.i04.com`. the text that I highlighted is the answer to number 2

![image](https://user-images.githubusercontent.com/81352414/198835005-1ef53d81-59cf-4357-b30d-dc58db751a7f.png)

this is for testing

![image](https://user-images.githubusercontent.com/81352414/198835116-1c644b99-7988-44a5-a320-e648c9c70cf1.png)

## 3. create a subdomain `eden.wise.yyy.com` with alias www.eden.wise.yyy.com whose DNS is set on WISE and leads to Eden

numbers 2 and 3 are almost the same, only the domains are different

the text that I highlighted is the answer to number 3

![image](https://user-images.githubusercontent.com/81352414/198835235-a7c36d73-c348-48ba-b889-ed2c0136495a.png)

## 4. create a reverse domain for the main domain

first we open it in wise then the text that I highlight is reverse dns

![image](https://user-images.githubusercontent.com/81352414/198835387-9a91b8cd-df7d-4574-8093-86685ed82c98.png)
![image](https://user-images.githubusercontent.com/81352414/198835512-0cef1c29-8f31-4cb8-9915-250d21fc8240.png)

make sure you have `dnsutils` installed, and then we testing 

![image](https://user-images.githubusercontent.com/81352414/198835581-664fe57b-59d6-49a5-a64c-47c0ace9faa1.png)

## 5. make Berlint also as the DNS Slave for the main domain

open berlint and do nano `/etc/bind/named.conf.local`

![image](https://user-images.githubusercontent.com/81352414/198835851-c155c8b4-2320-4364-95a1-13a1e6a9f0f1.png)

do `service bind9 stop` at wise

![image](https://user-images.githubusercontent.com/81352414/198836008-015c7fc7-2413-464e-8127-1152592f5721.png)

open sss and make sure there is an ip from wise and berlint

![image](https://user-images.githubusercontent.com/81352414/198836072-f989b500-8c71-4922-a9f5-ba101bbebea1.png)

ping the sss `www.wise.i04.com`, it will still connect, make sure wise is off because we have successfully created a slave

![image](https://user-images.githubusercontent.com/81352414/198836193-649452f3-e59d-4154-ab94-192168e7acd0.png)







