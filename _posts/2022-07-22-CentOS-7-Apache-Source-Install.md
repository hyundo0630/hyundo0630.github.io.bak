---
title : "[CentOS 7] Apache Source Install"
categories : 
    - CentOS
tags :
    - CentOS 7
    - Apache

toc: true
toc_sticky: true
---

## [CentOS7] Apache Source Install

테스트 환경<br>
  - OS : CentOS 7<br>
  - Apache Version : 2.4.6<br>

<li>Apache 설치 전, 서버 내부 Port 상태를 확인 해줍니다.</li><br>

```
# netstat -tlnp
```

<img src="https://github.com/hyundo0630/hyundo0630.github.io/blob/main/images/CentOS7%20netstat.png?raw=true"><br>

# 1. 필요한 패키지 다운로드 및 설치<br>
```
yum install -y wget expat-devel gcc gcc-c++
```
<li> wget = CLI(Command Line Interface) 환경에서 URL 을 이용한 파일 다운로드 Util</li>
<li> expat-devel = 1. Apache 설치 시 htpasswd error 발생 원인</li>
            2. expat을 가지고 XML 응용 프로그램을 개발하는데 필요한 Libary들과 File들
