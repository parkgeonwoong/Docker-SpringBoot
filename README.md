# Docker-SpringBoot


<p>
  <strong>• Stack</strong>&nbsp&nbsp&nbsp
<img src="http://img.shields.io/badge/Git-F05032?style&logo=Git&logoColor=white"/></a> &nbsp
<img src="http://img.shields.io/badge/Spring Boot-6DB33F?style&logo=Spring Boot&logoColor=white"/></a> &nbsp
<img src="http://img.shields.io/badge/Docker-2496ED?style&logo=Docker&logoColor=white"/></a> &nbsp
</p>

<p>
  <strong>• Environment</strong>&nbsp&nbsp&nbsp
<img src="http://img.shields.io/badge/Windows Terminal-4D4D4D?style&logo=Windows Terminal&logoColor=white"/></a> &nbsp
<img src="http://img.shields.io/badge/PowerShell-5391FE?style&logo=PowerShell&logoColor=white"/></a> &nbsp
<img src="http://img.shields.io/badge/Ubuntu-E95420?style&logo=Ubuntu&logoColor=white"/></a> &nbsp
<img src="http://img.shields.io/badge/NGINX-009639?style&logo=NGINX&logoColor=white"/></a> &nbsp
<img src="http://img.shields.io/badge/Apache Maven-C71A36?style&logo=Apache Maven&logoColor=white"/></a> &nbsp
</p>

<p>
  <strong>• IDE</strong>&nbsp&nbsp&nbsp
<img src="http://img.shields.io/badge/IntelliJ IDEA-000000?style&logo=IntelliJ IDEA&logoColor=white"/></a> &nbsp
</p>
<br />

## ✅ Installation
- [IntelliJ IDEA](https://www.jetbrains.com/ko-kr/idea/download/#section=windows)

IntelliJ IDEA is a cross-platform IDE that provides consistent experience on the Windows, macOS, and Linux operating systems.  
<br />

- Docker
  - [Ubuntu](https://docs.docker.com/engine/install/ubuntu/)  
    
    > Linux
    > 
    > The 3.10.x kernel is the minimum requirement for Docker.
  - [Window](https://docs.docker.com/docker-for-windows/install/)
  
    > Windows 10
    > 
    > Hyper-V must be enabled in BIOS VT-D must also be enabled if available (Intel Processors)  
    
  - DockerHub Repository Public Create
<br />

- Build: Maven
<br />


### 🔸 Usage
1. Dockfile
```bash
FROM openjdk:11
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]
```

2. Maven build & DockerImage
```bash
docker build -t DockerHubId/DockerRepository:TagName . 
```

3. Ubuntu Terminal
```bash
docker run -d -p 8080:8080 DockerHubId/DockerRepository:TagName
```

4. url: localhost:8080/
<br />


### 🔸Dependency
- thymeleaf
- web
- web-services
- test
<br />


#docker #SpringBoot
