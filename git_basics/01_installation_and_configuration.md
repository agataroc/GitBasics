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
