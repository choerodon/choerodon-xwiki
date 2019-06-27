该项目根据[XWiki扩展组件](https://www.xwiki.org/xwiki/bin/view/Documentation/DevGuide/Tutorials/WritingComponents/)创建，实现了文档`是否注释`、`收藏`和`分享功能`，并自定义[REST API](https://www.xwiki.org/xwiki/bin/view/Documentation/UserGuide/Features/XWikiRESTfulAPI)实现功能。

### 注意事项
1. 如果类继承了`HttpServlet`实现功能，需要在web.xml进行配置，如：
    ```
    <servlet>
        <servlet-name>CollectServlet</servlet-name>
        <servlet-class>io.choerodon.wiki.collect.api.servlet.CollectServlet</servlet-class>
    </servlet>

    <servlet-mapping>
        <servlet-name>CollectServlet</servlet-name>
        <url-pattern>/collect/*</url-pattern>
    </servlet-mapping>
    ```
2. 使用REST API实现功能需要在`components.txt`配置资源路径，API入口为`  http://host:port/rest`。
具体例子参考路径`choerodon-wiki-extention\choerodon-wiki-collect\src\main\java\io\choerodon\wiki\collect\app\service`。

