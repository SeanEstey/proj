


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
