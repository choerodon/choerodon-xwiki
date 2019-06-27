# 项目简介

本项目用于构建xwiki的docker镜像。基于[XWiki 10.4](https://github.com/xwiki-contrib/docker-xwiki)基础镜像构建。

- **agent**  [Skywalking调用链监控](http://skywalking.apache.org/zh/)
- **choerodon-xwiki**  包含XWiki所有的扩展以及初始化数据库sql
- **save** 快捷键`Ctrl + S`实现
- **choerodon-wiki-annotation.jar、choerodon-wiki-collect.jar、choerodon-wiki-share.jar** 文档注释、收藏、分享功能实现
- **comments.js** 评论提示是否为空功能实现
- **docker-entrypoint.sh** 主要增加了自定义了XWiki环境变量
- **hibernate.cfg.xml** hibernate配置
- **kotlin-stdlib-1.3.31.jar、okio-2.2.2.jar、okhttp-3.14.2.jar、minio-3.0.10.jar、google-http-client-1.20.0.jar、google-http-client-xml-1.20.0.jar** minio文件上传所需jar包

## 注意事项

如果镜像运行，提示`docker-entrypoint.sh`执行没有权限，请先执行`chmod`命令然后再打镜像。
