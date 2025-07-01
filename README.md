# Ansible Static Site Deployment

This repository contains an Ansible playbook to automate the installation of **NGINX** and the deployment of a simple static HTML page on a remote Linux server.

> 🧠 Built with 20+ years of industry experience in DevOps, automation, and infrastructure design.

---

## 📌 Project Objectives

- Automate the provisioning of a static web server using **Ansible**
- Install and configure **NGINX** via a secure and repeatable playbook
- Deploy a sample `index.html` file to `/var/www/html` on the target host
- Follow best practices in Ansible playbook design for clarity, reusability, and maintainability

---

## 🛠️ Technologies Used

- **Ansible**
- **NGINX**
- **Linux (Debian/Ubuntu)**
- **YAML**

---

## 🖼️ Live Page Preview

Below is a screenshot of the static site deployed using this Ansible playbook:

![Screenshot 2025-07-01 134331](https://github.com/user-attachments/assets/7aea0a9c-16be-4fcd-988d-330a3aa71676)



## 📁 Files Included

| File                          | Description                                |
|------------------------------|--------------------------------------------|
| `deploy_static_page_play.yml`| Ansible playbook to install nginx & deploy site |
| `index.html`                 | Sample static HTML homepage                |

---

## 🚀 How to Use

1. **Clone the repository** to your local machine:

    ```bash
    git clone git@github.com:Rahuljoshi07/ansible-static-site.git
    cd ansible-static-site
    ```

2. **Ensure you have Ansible installed**:

    ```bash
    sudo apt update
    sudo apt install ansible -y
    ```

3. **Define your inventory file** (e.g., `hosts.ini`):

    ```ini
    [server]
    your_remote_server_ip
    ```

4. **Run the playbook**:

    ```bash
    ansible-playbook deploy_static_page_play.yml -i hosts.ini -u your_user --ask-pass --ask-become-pass
    ```

---

## 📈 Scalability

This playbook is designed to be extended. You can easily:
- Add support for templated pages using `template` module
- Integrate CI/CD pipelines
- Add TLS/SSL with Let's Encrypt
- Deploy full front-end builds (React, Vue) into NGINX

---

## 🧑‍💼 Author

**Rahul Joshi**  
Senior DevOps Consultant  
📧 rj1342627@gmail.com  
🔗 [github.com/Rahuljoshi07](https://github.com/Rahuljoshi07)

---

## 📜 License

Feel free to use it and build on top of it.

---

> 💡 _Automation is not just about speed — it’s about consistency, confidence, and craftsmanship._
