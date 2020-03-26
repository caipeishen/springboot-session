

#### 解决的是同一个浏览器 不同服务(Tomcat)  Session共享

> 是以sessionID来区分

> 只需要加入Redis数据库配置，@EnableRedisHttpSession注解以及Manve依赖

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.session</groupId>
    <artifactId>spring-session-data-redis</artifactId>
</dependency>
```

