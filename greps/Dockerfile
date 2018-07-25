FROM tomcat 
ENV DIR_WEBAPP /usr/local/tomcat/webapps/
RUN  rm -rf $DIR_WEBAPP/*     #删除webapp下所有文件，因为当前应用作为根应用
ADD greps.war $DIR_WEBAPP/ROOT.war 
RUN  unzip $DIR_WEBAPP/ROOT.war  -d  $DIR_WEBAPP/ROOT/
CMD ["catalina.sh", "run"]
