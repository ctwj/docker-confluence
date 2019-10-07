# docker-confluence
confluence

```
docker run --detach --publish 8090:8090 ctwj/conflu
```

许可证
```
# 需替换邮箱（test@test.com）、名称（BAT）、
# 访问地址（http://192.168.0.89）、服务器ID（BY9B-GWD1-1C78-K2DE）
# 为你的信息

java -jar t.jar -d -m test@test.com -n BAT -p conf -o http://192.168.0.89 -s BY9B-GWD1-1C78-K2DE
```

t.jar
```
https://github.com/ctwj/docker-confluence/blob/master/t.jar
```


# docker-compose 部署

```
git clone https://github.com/ctwj/docker-confluence.git
cd docker-confluence/compose
docker-compose up -d
# 获取许可
docker exec -it conflu java -jar /opt/atlassian/confluence/t.jar -d -m ctwj@qq.com -n CTWJ -p conf -o http://192.168.0.89 -s BY9B-GWD1-1C78-K2DE
```
