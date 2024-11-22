# SSH key setup

Create .ssh
```bash
mkdir .ssh
```

cd into it
```bash
cd .ssh
```
Create key
```bash
ssh-keygen -t ed25519 -C email@adress
```
Add it to agent
```bash
eval "$(ssh-agent -s)"
```
```bash
ssh-add <keyname>
```
