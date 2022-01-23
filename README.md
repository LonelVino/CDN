# 免费CDN：jsDelivr+Github 使用方法

## 1.克隆Github仓库到本地

```bash
git clone https://github.com/LonelVino/CDN.git
## 进入仓库
cd CDN
```

## 2. 上传资源

复制需要上传的资源到本地git仓库（注：jsDelivr不支持加载超过20M的资源）

```bash
git status                    ##查看状态
git add .                     ##添加所有文件到暂存区
git commit -m '第一次提交'      ##把文件提交到仓库
git push                      ##推送至远程仓库
```

## 3.发布仓库

和平常不一样的重点来了 ：点击release发布

![image-20210521075834767](https://cdn.jsdelivr.net/gh/LonelVino/CDN@1.4.5/git-static/CDN_release.png)

## 4.通过jsDelivr引用资源

说了这么多，该怎么使用jsDelivr引用资源呢？

使用方法：

`https://cdn.jsdelivr.net/gh/你的用户名/你的仓库名@发布的版本号/文件路径`

例如：

```text
https://cdn.jsdelivr.net/gh/LonelVino/CDN@1.0/images/****.png
```

注意：版本号不是必需的，是为了区分新旧资源，如果不使用版本号，将会直接引用最新资源
