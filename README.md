# Cloudera   

## INSTALL
https://docs.cloudera.com/documentation/enterprise/5-13-x/topics/quickstart_docker_container.html    

##  Docker CDH单点架构


```
docker run -m 4G --memory-reservation 2G --memory-swap 8G      --hostname=quickstart.cloudera --privileged=true -t -i -d --publish-all=true  -p 8888:8888 -p 80:80 -p 7180:7180 -p 21050:21050 -p 50070:50070 -p 50075:50075 -p 50010:50010 -p 50020:50020 -p 8020:8020 5e0f9625ffee /usr/bin/docker-quickstart

```
参数解释：

```
docker run 
-m 4G --memory-reservation 2G --memory-swap 8G      
--hostname=quickstart.cloudera 
--privileged=true 
-t -i -d 
--publish-all=true  
-p 8888:8888 -p 80:80 -p 7180:7180 -p 21050:21050 
-p 50070:50070 -p 50075:50075 -p 50010:50010 -p 50020:50020 
-p 8020:8020 

5e0f9625ffee 

/usr/bin/docker-quickstart

```



```
/home/cloudera/cloudera-manager --express && service ntpd start
```



##  正确的启动方法：

```
先运行命令启动集群
docker  run  --hostname=quickstart.cloudera --privileged=true -t -i -d --publish-all=true  -p 8888:8888 -p 80:80 -p 7180:7180 -p 21050:21050 -p 50070:50070 -p 50075:50075 -p 50010:50010 -p 50020:50020 -p 8020:8020 5e0f9625ffee /usr/bin/docker-quickstart 



然后运行manager
/home/cloudera/cloudera-manager --express 

service ntpd start

```




https://xieshaohu.wordpress.com/2019/02/26/15%E5%88%86%E9%92%9F-%E5%9C%A8docker%E5%90%AF%E5%8A%A8cloudera%E5%B9%B6%E5%BC%80%E5%A7%8B%E4%BD%93%E9%AA%8C/    


https://www.cnblogs.com/piperck/p/9917118.html


## IMPALA    
![ ClouderaIMPALA](https://raw.githubusercontent.com/latermonk/Cloudera/master/_Image/impala-archtecture.jpg)

https://www.w3cschool.cn/impala/impala_overview.html   

## Cloudera Impala 常见问题
https://blog.csdn.net/weixin_35852328/article/details/83178299    


