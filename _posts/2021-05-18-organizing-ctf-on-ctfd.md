---
layout: post
title: How to Organize a CTF on CTFd for free?
tags: [CTF, Host CTF]
color: turquoise
excerpt_separator:
---

> *Digital Ocean provide free 100$ Credit to every new user for one time.*

[Digital Ocean](https://www.digitalocean.com/)

We are going to use this credits to host our ctf.
> *Note: You will get credits, only if you have Credit Card, International Debit Card or PayPal account.*

After creating the account, go to homepage and click on Get started with a Droplet.

![image](https://user-images.githubusercontent.com/47115503/120077390-db960900-c0c7-11eb-8131-9d8e5d19230a.png)

After this, you will get an option to choose OS. I will go for Ubuntu 18.4 (LTS) x64. Will config it to:
- 8 GB/ 4 CPUs
- 5 TB Transfer
- 160 GB SSD

![image](https://user-images.githubusercontent.com/47115503/120077407-f2d4f680-c0c7-11eb-8728-681bacdc9f5d.png)
![image](https://user-images.githubusercontent.com/47115503/120077411-f7011400-c0c7-11eb-89a0-0a46cb6b9115.png)

After choosing the plan, choose a datacenter region. Now, create a password for root.

![image](https://user-images.githubusercontent.com/47115503/120077424-008a7c00-c0c8-11eb-9464-b041f734123f.png)

Then, click on Create Droplet option. You will get your IP address once all done.

Now login into the machine with ssh.

> *Username: root Password: <You choosed>*

`apt update && apt upgrade`
Once update & upgrade is done. We have to install **docker** & **docker-compose**.
`apt install docker docker-compose`
All done? Visit ctfd deployment (docs) page to proceed.
[CTFd](https://docs.ctfd.io/docs/deployment/)

![image](https://user-images.githubusercontent.com/47115503/120077526-6b3bb780-c0c8-11eb-9bd6-913e7a9683c0.png)

Now open tmux session by typing `tmux`. Clone the ctfd repo first & then move forward.
```
git clone https://github.com/CTFd/CTFd.git
```
Move to CTFd dir and open **docker-compose.yml** file. Here, we have to update the secret key & workers (so that it can handle the load.)
After making changes, save & exit *docker-compose.yml* file. And type `docker-compose up`. It will start your ctfd. This may take few minutes. All done 👍

![image](https://user-images.githubusercontent.com/47115503/120077565-9920fc00-c0c8-11eb-865c-731f1322a8b9.png)
Now, visit [cloudflare](https://www.cloudflare.com/) website, add your website with a free plan [Basic]. Once the website is added successfully, add a record in DNS Management as follows:
> *Type: A Name: <subdomain> IPv4 Address: <IP Address>*

Just save it. Now visit your subdomain site and setup your admin account with other configurations.
Now sit back and enjoy 😉
