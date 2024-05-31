# Project #3 - Shinobi Application Deployment.

Project Type: Application Dockerization and Deployment on Kubernetes cluster.

Project Description: The client asked me to deploy Shinobi CCTV application on kubernetes cluster, MYSQL database should be connected to application. Configuration of Persistent volumes and persistent volume claims to store data, allocate 5gb memory to each volume.

Solution:
- I deployed PersistentVolume using NFS for Shinobi Applicaiton.
- I deployed PersistentVolume using NFS for MYSQL Database.
- I deployed PersistentVolume using NFS for Shinobi Livestreams.
- I deployed PersistentVolumeClaims for Shinobi, MYSQL, Streams.
- I deployed a Secret for Shinobi Applicaiton's Credentials.
- I deployed MYSQL Database Deployment and Service.
- I deployed Shinobi Application's Deployment and Service.
- I configured pre-requisites by connecting to Shinobi Application's pod.

![859bdeab5f8d42bc89cc05b838fa3908](https://github.com/awab-hassan/03-shinobiApplication-DEVOPS/assets/90965012/9e6f01a5-894e-4402-9b3f-0a1acbe2243d)
