## Configure New Ubuntu Instance

### Shell/Configs

Install fish shell

```
sudo apt install fish
chsh -s /usr/bin/fish
```

### Git Setup

#### Generate/Add SSH Key

```
ssh-keygen -t rsa -C estese@gmail.com
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/<key_name>
```

#### Create Repo

```
git init .
git add <file1> <file2>
git commit -am <comments>
git remote add origin git@github.com:SeanEstey/proj.git
git branch -M main
git push -u origin main
```

### MongoDB Setup

Open etc/mongod.conf

```
# network interfaces
net:
  port: 27017
    bindIp: 127.0.0.1,<internal_ip>       # run 'ip add' to find internal ip
```
