Spring Boot JSP Tutorial 
=============
   

등록일 : 2019.04.18
<hr/>

개발 환경
-------------
- gradle
  - Spring-boot 2.0.4  
  - Java 1.8 
  - spring-boot-starter-devtools 
  - spring-boot-starter-web
  - javax.servlet:jstl
  - tomcat-embed-jasper       
  
                 
- application.yml    


<pre><code>
server:
  port: 9090

spring:
   mvc:
    view:
      prefix: /WEB-INF/start/
      suffix: .jsp
</code></pre>


TestController 
-------------


<pre><code>
@RequestMapping("/")
public String index()
{
	return "index";
}
</code></pre>


실행
-------------
    curl http://localhost:9090/

