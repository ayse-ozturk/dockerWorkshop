# Docker Tutorials 
[Docker](https://docker.com/)
[GitHub Link](https://github.com/ayse-ozturk/dockerWorkshop)
[DockerHub](https://hub.docker.com/)

---


```sh
docker -v 
docker --version 
docker info
```

- Bare Metal
- Virtual Machine 
- Containerization 
- Docker gemi limanlarında gemilere yük taşıyan ve boşaltan  işcilere denir. 
- Docker 2008 --> Solomon Hykes 
- Şirket Adı: DotCloud --> Docker.INC
- go dilinde yazılır
- Docker aynı işletim sistemi ğzerinde birbirinden bağımsız ve izole container oluşturmamızı destekler 
- docker: Hızlı derleme, test için, dağıtım, ölçeklendirmeyi sağlar. 
- dockerHub: Docker imagelarının saklandığı yerdir. 
- 2015 --> Docker Swam eklenmiş 
- Farklı işletim sistemlerinde çalışıyor (Cross Platform)
- Docker CE 
- Docker EE
  ---


DockerHub: Docker imagelarımızı sakladığımız yer
Image: Bütün ayarları yapılmış çalışmayı beklenen docker objesidir. 
Container:Imageların çalıştığı yer
Dockerfile: image oluştumak için kullanılır. (docker build -t imageName)
docker-comnpose: Birden fazla servisin yönetildiği yerdir. (docker-compose up -d)
volume:Docker verilerinin kalıcılığı
swarm: docker orchestration(ölçeklendirme)
network:farklı Containerlerimizin birbiri ile bağlantı kurduğu alanlardır.
dockerize: Bir projeyi docker üzerinde koşturmak demektir

PORT
65536 port
Port 65536 port 0<=PORT<=1023 1024<=PORT<= 49151 49152<=PORT<=65535

**Docker info**
$ docker info
Client:
 Version:    27.0.3
 Context:    desktop-linux
 Debug Mode: false

Server:
 Containers: 0
  Running: 0
  Paused: 0
  Stopped: 0
 Images: 1
 Server Version: 27.0.3
 Storage Driver: overlayfs
  driver-type: io.containerd.snapshotter.v1
 Logging Driver: json-file
 Cgroup Driver: cgroupfs
 Cgroup Version: 1
 Plugins:
  Volume: local
  Network: bridge host ipvlan macvlan null overlay
  Log: awslogs fluentd gcplogs gelf journald json-file local splunk syslog
 Swarm: inactive
 Runtimes: io.containerd.runc.v2 runc
 Default Runtime: runc
 Init Binary: docker-init
 containerd version: ae71819c4f5e67bb4d5ae76a6b735f29cc25774e
 runc version: v1.1.13-0-g58aa920
 init version: de40ad0
 Security Options:
  seccomp
   Profile: unconfined
 Kernel Version: 5.15.153.1-microsoft-standard-WSL2
 Operating System: Docker Desktop
 OSType: linux
 Architecture: x86_64
 CPUs: 8
 Total Memory: 7.707GiB
 Name: docker-desktop
 ID: bb472ab1-35ca-498e-b67a-2c532e40591a
 Docker Root Dir: /var/lib/docker
 Debug Mode: false
 HTTP Proxy: http.docker.internal:3128
 HTTPS Proxy: http.docker.internal:3128
 No Proxy: hubproxy.docker.internal
 Labels:
  com.docker.desktop.address=npipe://\\.\pipe\docker_cli
 Experimental: false
 Insecure Registries:
  hubproxy.docker.internal:5555
  127.0.0.0/8
 Live Restore Enabled: false

