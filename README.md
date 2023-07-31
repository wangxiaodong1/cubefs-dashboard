# cubefs-dashboard
# cubefs-dashboard

Introduction
cubefs Console (cfs-gui) is a graphical management tool for cubeFS system, which is designed to meet the needs of system administrators and ordinary users for daily file management. It is an independent web service that is more intuitive and easier to get started with than cfs-cli.

Architecture
The cfs-gui backend interacts directly with the CubeFS cluster, manages multiple clusters simultaneously, and stores its own data in the database. The permission module can assign accounts to different application scenarios. cfs-gui has four main functional modules, as follows:
Virtual resource management: volume, data partition, metadata partition, erasure code strip
Physical resource management: nodes, disks, etc
Rights management: users and roles
File management: list, upload, download

<img src="https://github.com/cubefs/cubefs-dashboard/blob/main/pictures/architecture.png" align=center/>

Features
Managing multiple clusters: The Management Console is deployed independently of a cluster and can manage multiple clusters simultaneously
Flexible rights management: Console users can associate multiple roles, each role corresponds to a group of rights, each rights refers to an important button on the page
Volume creation and authorization: It allows you to create volumes and grant read and write permissions to tenants
Resource migration: The Console supports partition, disk, and machine dimension offline (automatic migration)/migration
File management: List, upload, download

Compilation
Requirements:
node version: v12-v14
npm version: the npm in node package
go version: v1.16 and later

# clone code
git clone https://github.com/cubefs/cubefs-dashboard.git

# build
make

# product
ll bin/
total 26256
-rwxr-xr-x 1 root root 26876984 Jul 27 17:26 cfs-gui
-rw-r--r-- 1 root root     1009 Jul 27 17:26 config.yml
drwxr-xr-x 6 root root     4096 Jul 27 17:27 dist

Preview
Cluster overview
图片: 
图片: 
图片: 


