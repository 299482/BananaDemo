��װ׼����
1.���ز���װJDK,JDK�汾ʹ��1.8+��jdk1.8.0_51
2.���ز���ѹApache Tomcat 7 or Tomcat 8; �� /opt/apache-tomcat-7.0.63;
3.��WebRoot����ΪLogAnalyzer���������� /opt/apache-tomcat-7.0.63/webapps�£���/opt/apache-tomcat-7.0.63/webapps/LogAnalyzer
4.���������ļ�Ŀ¼��/opt/apache-tomcat-7.0.63/logconf/
5.��dependent_jars_list�е�jar�ļ�������/opt/apache-tomcat-7.0.63/webapps/LogAnalyzer/WEB-INF/libĿ¼��
6.��scriptsĿ¼�µ�shell�ű�������/opt/apache-tomcat-7.0.63/binĿ¼�£���ִ�� chmod u+x *.sh

�ű��޸�
#/opt/apache-tomcat-7.0.63/lbin/setenv.sh�н�JAVA_HOME���ó�jdk��װ·����JDK�汾ʹ��1.8+
export JAVA_HOME=/opt/huawei/Bigdata/jdk1.8.0_51/

���ã�
1. ��HBase�ͻ��˵������ļ�core-site.xml��hbase-site.xml��hdfs-site.xml������/opt/apache-tomcat-7.0.63/webapps/LogAnalyzer/WEB-INF/classesĿ¼��
2.����krb5.conf��Ӧ���˻�keytab�ļ�������tomcat��װ·��logconfĿ¼�£����޸��޸�/opt/apache-tomcat-7.0.63/logconf/logconf.properties��Ӧ����
user.principal=
keytab.file.path=
krb5.conf.path=
3.�޸�tomcat��װ·��/opt/apache-tomcat-7.0.63/logconf/logconf.properties
#zkHosts����ֵ�ɵ�¼Solr Admin UI��ȡ��
solr.zkHost=192.168.213.6:24002,192.168.213.5:24002,192.168.213.4:24002/solr
#IP�滻��SolrAdmin�ĸ���IP
search.server.url=https://192.168.213.44:21101/solr/ 
