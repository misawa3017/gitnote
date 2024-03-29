# git教學

![git原理](https://github.com/misawa3017/gitnote/blob/main/git_principle.png)


## git初始化 new repo

```bash
git config --global user.name "user"
```

```bash
git config --global user.email "user@gmail.com"
```

```bash
echo "# bashnote" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/misawa3017/bashnote.git
git push -u origin main
```

## 更新遠端repo url
```bash
git remote set-url origin git@github.com:misawa3017/config.git
```
## 上傳已存在的repo

```bash
git remote add origin https://github.com/misawa3017/bashnote.git
git branch -M main
git push -u origin main
```

## 新增分支並切換分支

```bash
git checkout -b 1110308
```

## git clone 後，切換遠端分支
```bash
git fetch
git checkout <遠端分支>
```
## git merge 假如要master 要合併<要被合併的分支>
```bash
git checkout master
git merge <要被合併的分支>
git push
```

## git 刪除分支
```bash
git branch -d <branch>
```
## reset 本地並同步遠端
```bash
git fetch
git reset --hard HEAD
git merge origin/$CURRENT_BRANCH
```

### 假如你原本新增一個檔案並add to staging 後反悔
```bash
git restore --staged a.sh
git status
```

### 也可以執行這個指令
```bash
git reset HEAD
```