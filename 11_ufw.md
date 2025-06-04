
# 🛡️ What is UFW Firewall?

**UFW** stands for **Uncomplicated Firewall**. Think of it like a security guard for your Linux system.

## 🔒 Real-life Example

Imagine your laptop is a house. This house has many doors and windows (called **ports** in computer terms). Each door leads to a different room — one might be for your email, one for your browser, one for file sharing, and so on.

Now, you don’t want just anyone walking into any room. So you hire a security guard (**UFW**) to:

- Only allow your friends (trusted apps or IP addresses) to enter specific rooms.
- Block strangers (unwanted connections) from accessing the house.
- Watch the gates and report any suspicious activity.

## 🔧 Why Use UFW?

- It’s easy to use, even for beginners.
- It adds a layer of protection to your server or computer.
- It helps prevent hackers from accessing your system.

## 🛠️ Common UFW Commands

| Command | What it does |
|---------|----------------|
| `sudo ufw status` | Check if the firewall is on and what rules are active. |
| `sudo ufw enable` | Turn on the firewall (like telling the guard to start working). |
| `sudo ufw disable` | Turn off the firewall (the guard takes a break — not recommended). |
| `sudo ufw allow 22` | Allow door/port 22 (used for SSH remote login). |
| `sudo ufw deny 80` | Block door/port 80 (used for websites). |
| `sudo ufw delete allow 22` | Remove the rule that allows port 22. |
| `sudo ufw reset` | Remove all rules and start fresh. |
| `sudo ufw allow from 192.168.1.10` | Only allow this specific IP to access. |

## 🚪 Common Ports You Should Know

| Port | Service | Why it's used |
|------|---------|----------------|
| 22   | SSH     | For connecting to your server remotely |
| 80   | HTTP    | Regular websites (non-secure) |
| 443  | HTTPS   | Secure websites |
| 3306 | MySQL   | Used by databases |

## ✅ Sample Workflow

When setting up a server:

1. Enable UFW: `sudo ufw enable`
2. Allow SSH so you can connect: `sudo ufw allow 22`
3. Allow web traffic (if you're hosting a site): `sudo ufw allow 80` and `sudo ufw allow 443`
4. Check the rules: `sudo ufw status`

## 🧠 Final Tip (Golden Rule)

**Only open what you need.**  
If you're not using a service, don't leave the port open — it's like leaving your door unlocked.
