# AWS EC2 Static Website Deployment

## Project Overview
This project demonstrates the deployment of a **publicly accessible static website** on an **AWS EC2 instance** using **Amazon Linux** and **Nginx**.

The goal was to go beyond local testing and ensure the website could be accessed externally, simulating a real production-style deployment.

---

## Live Demo
🌐 **Public IP:**  
http://3.224.147.123/

---

## Technologies Used
- **AWS EC2** – Virtual server hosting the website
- **Amazon Linux 2023** – Operating system
- **Nginx** – Web server for serving static files
- **HTML & CSS** – Website structure and styling
- **SSH** – Secure remote server access
- **AWS Security Groups** – Network access control

---

## Deployment Steps
1. Launched an EC2 Free Tier instance running Amazon Linux.
2. Connected to the instance via SSH using a key pair.
3. Installed and configured Nginx using `dnf`.
4. Configured security groups to allow:
   - SSH (port 22) from my IP
   - HTTP (port 80) from anywhere
5. Deployed the static website files to: /usr/share/nginx/html
6. Restarted Nginx and verified external access using the public IP.

---

## Challenges & Learnings
- Adjusted commands for Amazon Linux 2023 (no `amazon-linux-extras`).
- Learned how file permissions and directory paths affect static deployments.
- Observed how browser caching can delay visible changes.
- Reinforced the importance of verifying deployments from an external browser.

---

## Key Takeaways
- Deployment confidence improves with repetition.
- Nginx is a reliable solution for serving static content.
- Small projects encourage production-level and DevOps thinking.
- A project is not complete until it is externally accessible.

---

## Author
Deployed and maintained by **Taiwo Badmus**
