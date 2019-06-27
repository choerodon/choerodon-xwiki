FROM xwiki:10.4-mysql-tomcat

ADD docker-entrypoint.sh /usr/local/bin/
ADD xwiki.properties /usr/local/tomcat/webapps/ROOT/WEB-INF/
ADD setenv.sh /usr/local/tomcat/bin/
ADD choerodon-xwiki /root/data/
COPY hibernate.cfg.xml /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml
ADD web.xml /usr/local/tomcat/webapps/ROOT/WEB-INF/
ADD choerodon-wiki-collect.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD choerodon-wiki-share.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD choerodon-wiki-annotation.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD xwiki-platform-legacy-oldcore-10.4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD agent /agent
ADD save /usr/local/tomcat/webapps/ROOT/resources/save
ADD comments.js /usr/local/tomcat/webapps/ROOT/resources/uicomponents/viewers
ADD logback.xml /usr/local/tomcat/webapps/ROOT/WEB-INF/classes
ADD kotlin-stdlib-1.3.31.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD okio-2.2.2.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD okhttp-3.14.2.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD minio-3.0.10.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD google-http-client-1.20.0.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib
ADD google-http-client-xml-1.20.0.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib