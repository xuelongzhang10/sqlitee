# sqlitee
自己写的第一个，spring boot sqlite jpa

更新一下gradle版本的配置文件：
首先是application.yaml
 spring:
  jpa:
    hibernate:
      ddl-auto: update
    database-platform: com.vivedu.cls.config.SQLiteDialect    //这是项目中SQLiteDialect的地址
    show-sql: true
  datasource:
    url: jdbc:sqlite:D:/Studio/LocalServer_dev/db/data.db     //这是指定生成db文件的位置
    driver-class-name: org.sqlite.JDBC
    username:
    password:
然后是build.gradle
 compile 'org.xerial:sqlite-jdbc:3.8.11.2'
