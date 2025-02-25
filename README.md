# Add-DNS-to-Unicorn

How to link your DNS domain (i.e. www.community.com) to your Unicorn community.


## Steps

### 1. Enable DNSSEC
Open your registrar or hosting provider page and enable DNSSEC for your chose domain. Usually a setting or button under DNS.


### 2. Find your Domain in the ENS Manager

a. a. Open the ENS Manager App, connect your wallet, search for your DNS domain name and click on it to continue. You’ll see a page like the one below.

![image](https://github.com/user-attachments/assets/8d41660d-2896-4ea4-b2ac-6a91c2046a54)

b. Choose import onchain. Thhis will create an NFT of the domain for added proof of ownership and enable you to mint subdomains for your members.

You may need to wait until DNSSEC is marked as enabled -  usually it takes no longer that 15 mins for DNSSEC to propagate but it can take up to an hour.

![image](https://github.com/user-attachments/assets/e5a867cd-3969-4d99-aad0-b1650626d7ed)



### 3. Add Records in your Registrar or Hosting Provider

Navigate to your registrar or hosting provider's management interface and press “Add Record”.

a. Add a TXT-record to prove ownership of your domain name: 
Type: TXT
Name/Record: _ens
Value: a=your wallet address (i.e. a=0xae5D0....768A4)

Alternatively you can copy the record Type, Name, and Value from the ENS App (as seen below).

![image](https://github.com/user-attachments/assets/074ba677-b90d-4c31-999f-0ba42fdf45d2)

b. Then, add a CNAME-record to deploy your Unicorn app to your domain:
Type: CNAME
Name/Record: app
Value: saas.unicorn-account.com


### 4. Claim your Domain in the ENS App

Go back to the ENS Manager App and claim your now tokenised domain by pressing Register. Follow the instruction on the ENS App to sign and confirm the registration transaction on your wallet (includes paying registration and network fees in ETH).

Usually it takes no longer that 15 mins for records to update but it can take up to an hour.

![image](https://github.com/user-attachments/assets/bd9191fb-551d-4084-ba07-94973cdf8c68)

### 5. Li﻿nking your Domain to your Unicorn community

When steps 1-4 have been completed reach out to the Unicorn to link the webapp to your domain.
