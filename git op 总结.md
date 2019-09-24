# git op
---
## 1. 拉取远程分支，修改后提交
[1] git clone xxx
```git
git clone xxx.git
```
[2] 查看远程分支
```git
git branch -r 
```
[3] 拉取远程分支
```git
git pull origin name_remote:name_local
```
[4] 修改
```git
git checkout name_local
```
[5] add commit
```git
git add .
git commit -m "change branch name_remote"
```
[6] push
```git
git push origin name_local:name_remote
```

## Pull branch of remote
```git
git clone -b <branch> <remote_repo>
```

Example:
```git
git clone -b my-branch git@github.com:user/myproject.git
```
With Git 1.7.10 and later, add --single-branch to prevent fetching of all branches. Example, with OpenCV 2.4 branch:
```git
git clone -b opencv-2.4 --single-branch https://github.com/Itseez/opencv.git
```