# Installation & configuration

## Check Git Version
Displays the installed Git version.
```bash
git --version
```
## Configure Git (only the first time)
Sets a global identity.
```bash
git config --global user.name "Name"
git config --global user.email "your@email.com"
```
Verify configuration:
```bash
git config --list
```
---

GitLab *will* ask for your username and password every time you'll push or commit. If you don't want it to, you can either use:

## SSH Autentication (GitLab)
To generate a ne key(first time):
```bash
ssh-keygen -t rsa -b 2048 -C "<comment>"
```
The comment could be anything, even just your username. This will generate your ```id_rsa``` (private key) and ```id_rsa.pub``` (public key). Take the ```./ssh/id_rsa.pub``` content and paste it in GitLab WebUI (Profile > SSH Keys (https://gitlab.com/-/profile/keys)) as new SSH key. Now update your git origin to use SSH. If in your poject ```git remote -v```, you see something like ```https://gitlab.com/username/progetto.git```, you can change it with:
```bash
git remote set-url origin git@gitlab.com:username/progetto.git
```
---
# SSH Authentication (GitHub)(Recommended)

## Generate SSH Key

```bash
ssh-keygen -t ed25519 -C "your@email.com"
```

---

## Change Remote to SSH

```bash
git remote set-url origin git@github.com:username/repository.git
```
