---
title : "[CentOS 7] Apache Install"
categories : 
    - CentOS
tags :
    - CentOS 7
    - Apache

toc: true
toc_sticky: true
---

## [CentOS7] Apache Install

테스트 환경
    - OS : CentOS 7
    - Apache Version : 2.4.6

<li>Apache 설치 전, 서버 내부 Port 상태를 확인 해줍니다.</li>
```
# netstat -tlnp
```
<img src="https://github.com/hyundo0630/hyundo0630.github.io/blob/main/images/CentOS7%20netstat.png?raw=true">

# 1. Apache Install
```
yum install httpd httpd-devel
```
