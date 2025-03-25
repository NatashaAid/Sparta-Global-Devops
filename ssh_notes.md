# SSH Notes

## What is SSH?

**SSH (Secure Shell)** is a protocol used to securely access remote systems. Regarding Git and GitHub, it allows you to authenticate and push code without entering your username and password each time.

## What is an SSH Key Pair?

An SSH key pair includes:

- A **private key** (kept on your local machine and never shared)
- A **public key** (uploaded to GitHub or other remote services)

The private key proves your identity, and the public key tells the service it's safe to trust your machine.

## Common SSH Commands

- `ssh-keygen -t rsa -b 4096 -C "your-email@example.com"` – Generate a new SSH key
- `eval $(ssh-agent -s)` – Start the SSH agent
- `ssh-add <key-name>` – Add your private key to the agent
- `cat <key-name>.pub` – Show your public key to copy and add to GitHub
- `ssh -T git@github.com` – Test your SSH connection

## Key Reminders

- Only ever share your **public key** (`.pub` file)
- Keep **private key** secure and never commit it to a repository
- Once set up, SSH allows passwordless secure communication with GitHub

## When to Use SSH

- When cloning/pushing to private repos
- To avoid repeatedly typing your GitHub login
- As a more secure alternative to HTTPS authentication
