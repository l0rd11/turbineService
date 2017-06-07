# turbineService

## Description
turbineService is a turbine microservice for sius course.

### Starting
```
$ gradlew bootRun
```
first start eureka service and config service and rabbitMq with folowing config first time starting:
```
sudo rabbitmq-server
sudo rabbitmq-plugins enable rabbitmq_management
sudo rabbitmqctl add_user admin admin
sudo rabbitmqctl set_permissions admin  ”.*” ”.*” ”.*”
sudo rabbitmqctl set_user_tags admin administrator
```
normal start
```
sudo rabbitmq-server
```
After running, use this url in the hystrix dashboard: http://localhost:8981/turbine.stream
