# Wildfly

This is a Wildfly Container based on the offical jboss/wildfly Image. An user with the following privileges is created:

```
username: admin
password: admin
```

<img src="http://design.jboss.org/wildfly/logo/final/wildfly_logo_450px.png"/>


## Installation

```
docker pull renewinkler/wildfly
```

## Launch

```
docker run -itd -p 8080:8080 --name wildfly renewinkler/wildfly
```

## Launch with Admin Console

``` 
docker run -p 8080:8080 -p 9990:9990 -d --name wildfly_admin renewinkler/wildfly
```

## Usage

```
Application: http://192.168.99.100

Admin Console: http://192.168.99.100:9990/
```


## Connect to Server

```
docker exec -it wildfly_admin /bin/bash
```

