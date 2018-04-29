## 如何使用hexo的部署功能
使用`hexo d -g`可以自动生成网站并且推送到GitHub上，前提是安装一个软件包,并且在`_config.yml`中配置git的ssh地址：
```
npm install hexo-deployer-git --save
```

## 如何拉去主题仓库
如果是第一次，首先添加子模块，如下所示：
```
git submodule add -b card https://github.com/yscoder/hexo-theme-indigo.git themes/indigo
```

后续只需要更新主题代码即可：
```
git submodule init 
git submodule update
```