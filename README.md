# spring-connection-pool-imple-hikari-cp-
Hikari CP implementation 

```
#-----------------------------------
# Connection Pool configuration using HikariCP
#-----------------------------------
spring.datasource.hikari.poolName=auth-service-localhost-cp
#defines connection pool name
spring.datasource.hikari.connection-timeout = 30000
#maximum number of milliseconds that a client will wait for a connection
spring.datasource.hikari.minimum-idle= 5
#minimum number of idle connections maintained by HikariCP in a connection pool
spring.datasource.hikari.maximum-pool-size= 10
#maximum pool sizespring.datasource.hikari.idle-timeout=10000 
#maximum idle time for connection
spring.datasource.hikari.max-lifetime= 60000 
# maximum lifetime in milliseconds of a connection in the pool after it is closed.
spring.datasource.hikari.auto-commit =true 
#default auto-commit behavior.

 

#-----------------------------------
# Connection Pool Logs configuration - HikariCP
#If a deeper level of details are needed then replace DEBUG with TRACE.
#-----------------------------------
logging.level.com.zaxxer.hikari.HikariConfig=DEBUG 
logging.level.com.zaxxer.hikari=DEBUG 
# Actuator-metrics Configuration
management.endpoint.metrics.enabled = true
management.endpoints.web.exposure.include = metrics
```

## Reference links 
https://www.javadevjournal.com/spring-boot/spring-boot-hikari/

https://stackoverflow.com/questions/60757590/logging-hikaricp-spring-boot

https://www.masterspringboot.com/data-access/jpa-applications/hikari-connection-pool-with-spring-boot-made-simple/
