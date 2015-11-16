RabbitMQ Cloud Foundry Samples
==============================

This repository contains sample applications to demonstrate the use of [RabbitMQ](http://www.rabbitmq.com/) on [Cloud Foundry](http://www.cloudfoundry.com).

Examples are provided for the following languages/runtimes: 

* [Java with Spring](spring)
* [Ruby with Rails](rails)
* [Ruby with Sinatra](sinatra)
* [Node.js](nodejs)

```
manifest generator  : http://cfmanigen.mybluemix.net/?cm_mc_uid=42310564502714249767841&cm_mc_sid_50200000=1447697218
@@@@ start of manifest @@@
---
applications:
- name: rabbitmq-spring
  memory: 512M
  instances: 1
  host: rabbitmq-spring-${random-word}
  path: target/rabbitmq-spring-1.0-SNAPSHOT.war
  services:
  - cloudamqp
@@@ end of manifest
```
