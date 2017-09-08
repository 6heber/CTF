# PhrackCTF-Platform-Personal
   
虽然我不能保证这是前端最炫的CTF平台，但我相信这会是后台功能最友好的CTF平台。

Based on Spring and SpringMVC framework.


## Techniques

### Base Framework
spring & spring MVC
### Database Connect Pool:
Alibaba Druid
### SQL mapper framework
Mybatis
### Security framework
Apache Shrio

### Database
postgresql-9.5

### FrontEnd
Bootstrap & jQuery

## Notice
It's highly recommanded to use https when deploy this platform.  
Before using :  
1. Install umeditor maven dependencies commons-fileupload-1.2.2.jar and ueditor-mini.jar in src/main/webapp/umeditor/jsp to local Maven repository:   
**mvn install:install-file -Dfile=path_to_umeditor_mini_jar\ueditor-mini.jar -DgroupId=umeditor -DartifactId=ueditor-mini -Dversion=1.2.2 -Dpackaging=jar -DgeneratePom=true -DcreateChecksum=true**   
**mvn install:install-file -Dfile=path_to_commons_fileupload_jar\commons-fileupload-1.2.2.jar -DgroupId=umeditor -DartifactId=commons-fileupload -Dversion=1.2.2 -Dpackaging=jar -DgeneratePom=true -DcreateChecksum=true**   
2. Set mail server info in resources/spring-mail.xml because this platform using mail system to activate user.   
3. Set database information in system.properties   
4. Mail template in mail.properties
5. Create a user and set column "role" to "admin" for setting a user as administrator.     
