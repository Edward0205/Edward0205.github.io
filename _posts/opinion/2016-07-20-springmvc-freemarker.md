---
layout: post
title: �SpringMVC-Freemarker-Tomcat����
category: opinion
description: �SpringMVC-Freemarker-Tomcat����
---

    �������Ҫ��æ����һ���򵥵�Portal��Ŀǰ������SpringMVC+Freemarker+Tomcat���һ������������
##����׼��:
    1.Maven [Maven](http://maven.apache.org)
	2.Tomcat [Tomcat](http://tomcat.apache.org/index.html)

##ʹ��Eclipse����Web��Ŀ
    �������ֱ����maven��webappģ��������һ����Ŀ������������̫ϲ�����ַ�ʽ�������������һ�ַ�ʽ
	###1.�½�Maven Project
	![Create-1](http://www.liangye.info/images/springmvc/create-1.png)
	![Create-2](http://www.liangye.info/images/springmvc/create-2.png)
	����Ȼ����next��Ȼ������Լ����д��Group Id��Artifact Id�����Finish����
	
	###2.��Maven Projectת����Maven Web Project
	�Ҽ���Ŀ-Properties-Project Facets������ͼ��ʾ����ѡ�����ѡ����漴��
	![Create-3](http://www.liangye.info/images/springmvc/create-3.png)
	���Կ�����Ŀ�ṹ���£�
	![Create-4](http://www.liangye.info/images/springmvc/create-4.png)
	�����WebContent���ݣ�WebContent������Tomcat�в�����Ŀʱ��ĸ�Ŀ¼��
	
	������ϲ������һ����ͨ�ļ�����ʽ�Ķ��������Ҳ�������������һ�£��ⲽ���Թ�������Ȥ�����ѿ��Կ���
	
	�Ҽ���Ŀ-new-Source Floder�������µ�Դ���ļ��У��ļ�����������ȡsrc/main/webapp
	������src/main/webappȡ��WebContent��
	�Ҽ���Ŀ-Build Path-Configure Build Path
	![Create-5](http://www.liangye.info/images/springmvc/create-5.png)
	Ȼ����src/main/webapp�´����ļ���WEB-INF��������WEB-INF���洴��web.xml,web.xml��������:
	
	`
	<?xml version="1.0" encoding="UTF-8"?>
        <web-app version="2.5" xmlns="http://java.sun.com/xml/ns/javaee"
		xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
		xsi:schemaLocation="http://java.sun.com/xml/ns/javaee 
		http://java.sun.com/xml/ns/javaee/web-app_2_5.xsd">

		<welcome-file-list>
			<welcome-file>index.jsp</welcome-file>
	    </welcome-file-list>
    </web-app> 
    `
	����Web Project�ļ��ӻ����ǹ�����,�ṹ����ͼ��
	![Create-6](http://www.liangye.info/images/springmvc/create-6.png)