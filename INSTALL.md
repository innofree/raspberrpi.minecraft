# Raspberrypi Minecraft Server 세팅

### 원격 접속을 위해서 sshd 설치
```
root@raspberrypi:~# apt-get install openssh-server
```

### sshd 재시작
```
root@raspberrypi:~# service ssh restart
```

### 서비스 상태 확인
```
root@raspberrypi:~# netstat -natp
Active Internet connections (servers and established)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 127.0.0.1:5939          0.0.0.0:*               LISTEN      1589/teamviewerd
tcp        0      0 0.0.0.0:22              0.0.0.0:*               LISTEN      1849/sshd       
tcp        0      0 220.117.121.173:56470   159.8.67.132:5938       ESTABLISHED 1589/teamviewerd
tcp        0      0 127.0.0.1:5939          127.0.0.1:59308         ESTABLISHED 1589/teamviewerd
tcp        0      0 127.0.0.1:59308         127.0.0.1:5939          ESTABLISHED 1628/TeamViewer 
tcp6       0      0 :::22                   :::*                    LISTEN      1849/sshd       
root@raspberrypi:~# 

```

