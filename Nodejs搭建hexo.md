# 1.看版本号

```
node -v
npm -v
```

# 2.安装淘宝镜像源

```
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

# 3.安装hexo-cli

```
cnpm install -g hexo-cli

验证是否安装
hexo -v
```

# 4.搭建

```
pwd  :看路径
mkdir blog ：新建
cd blog
hexo init ：初始化博客
ls -l
hexo s ：启动
```

# 5.写文章

```
hexo new "My New" ：new文章
cd source/_posts/
ls -l
vim My New.md
```

# 6.配置

```
cd ../.. ：到blog目录
hexo clean ：清除一下
hexo g ：生成
hexo s ：运行
```

# 7.推到远端

```
GitHub新建仓库：Davis-Samuel.github.io

pwd  :到此目录下
/d/MY/已安装/Nodejs/blog

cnpm install --save hexo-deployer-git  ：下载远端工具

vim _config.yml ：修改配置文件
deploy:
  type: git
  repo: https://github.com/Davis-Samuel/Davis-Samuel.github.io.git
  branch: master
  
hexo d  ：部署远端

```

# 8.换主题

```
网址：github.com/litten/hexo-theme-yilia

pwd  :到此目录下
/d/MY/已安装/Nodejs/blog

克隆到themes/yilia
git clone https://github.com/litten/hexo-theme-yilia.git themes/yilia

pwd
ls -l
cd themes/
ls -l
cd ..  ：回到_config.yml文件

vim _config.yml ：修改配置文件
themes: yilia

:wq

hexo clean
hexo g
hexo d :推到远端
```

