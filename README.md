# git教學

## git初始化 new repo

```bash
git config --global user.name "misawa3017"
```

```bash
git config --global user.email "misawa3017@gmail"
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
