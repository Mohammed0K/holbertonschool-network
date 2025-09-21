# Networking basics #1

**Level:** Amateur  
**Author:** Sylvain Kalache  
**Weight:** 1  

---

## 📖 Description
This project builds on the basics of networking introduced in **Networking basics #0**.  
Here, we dive into concepts like **localhost**, `0.0.0.0`, the **hosts file**, and practical use of tools such as `ifconfig`, `nc`, and `telnet`.  
You will also practice configuring IP resolution, displaying active interfaces, and creating a listening port.

---

## 📚 Resources
Read or watch:
- What is localhost
- What is 0.0.0.0
- What is the hosts file
- Netcat examples

Man pages or help:
- `ifconfig`
- `telnet`
- `nc`
- `cut`

---

## 🎯 Learning Objectives
At the end of this project, you should be able to explain:

### General
- What is **localhost / 127.0.0.1**
- What is **0.0.0.0**
- What is **/etc/hosts**
- How to display your machine’s active network interfaces

---

## 📝 Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- All files interpreted on **Ubuntu 22.04**
- All files must end with a new line
- `README.md` file is mandatory at project root
- Bash script files must:
  - Be executable
  - Pass `Shellcheck` (version 0.7.0) without errors
  - Start with `#!/usr/bin/env bash`
  - Include a comment on the second line explaining the script

---

## 🧩 Tasks

### 0. Change your home IP
- Write a Bash script that:
  - Configures `localhost` to resolve to `127.0.0.2`
  - Configures `facebook.com` to resolve to `8.8.8.8`
- Uses `/etc/hosts` to override DNS.

**File:** `0-change_your_home_IP`

⚠️ **Note:** Revert `localhost` back to `127.0.0.1` after testing to avoid breaking system functionality.

---

### 1. Show attached IPs
- Write a Bash script to display all active IPv4 IPs of the machine.

Example:

```
./1-show_attached_IPs
10.0.2.15
127.0.0.1
File: 1-show_attached_IPs
```

2. Port listening on localhost

Write a Bash script that listens on port 98 on localhost.

Can be tested with telnet localhost 98.

Example:
```
telnet localhost 98
Hello world
```

---

📂 Repository Structure

holbertonschool-network/
└── basics_1/
    ├── 0-change_your_home_IP
    ├── 1-show_attached_IPs
    ├── 2-port_listening_on_localhost
    └── README.md

---

✅ Usage

Examples:

# Change IP mappings
sudo ./0-change_your_home_IP

# Show machine IPs
./1-show_attached_IPs

# Listen on port 98
sudo ./2-port_listening_on_localhost

---

📌 Notes

localhost (127.0.0.1) is the standard loopback interface.

0.0.0.0 means “all IPv4 addresses on the local machine.”

/etc/hosts file allows overriding DNS for testing and debugging.

nc and telnet are useful for testing connections and sockets.