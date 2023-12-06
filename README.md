# [ARGON EON SCRIPT ](https://argon40.com/blogs/argon-resources/argon-eon-installation-manual)
```
curl https://download.argon40.com/argoneon.sh | bash
```
```
sudo apt update && sudo apt upgrade -y
```

# [OMV INSTALL SCRIPT](https://github.com/OpenMediaVault-Plugin-Developers/installScript) 
```
sudo curl -sSL https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install | sudo bash
```

# [OMV ISSUES](https://github.com/openmediavault/openmediavault/issues)

# DELETE ALL FILES IN DIRECTORY
```
cd /srv/dev-disk-by-uuid-2c9a9967-2bc8-4515-92f8-40e23d90ea3b/ssd/docker\ data/jdownloader/output
```
```
rm -r *
```

# OMV6-DOCKER 

> I found most of the guide are based on portainer and after some trial and error... It seems working, here is the guide for my own reference when I started to use jdownloader in docker.

1. Install plugins ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/5bcbc8cf-f578-4969-a4c6-5bbaf416990d)
2. Enable docker repo in omv-extras ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/45dbee11-e155-481f-9686-f5b7335203bd)
3. Reboot OMV
4. After reboot - services - compose - settings - default storage can be changed based on user preferences ... youtube have many video guides for this, I referred to this https://www.youtube.com/watch?v=y-OWVwpoGow&t=0s (setup omv and share folders)
5. https://www.youtube.com/watch?v=1ICHdvSGHVs (setup docker / portainer in omv)
6. OMV have "add from example" and you just need to edit your desired path ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/bf031af7-f32a-4261-9b43-588a46b1738b)
7. Edit some parameter by following the quick start - https://hub.docker.com/r/jlesage/jdownloader-2#:~:text=time%20every%20day!-,Quick%20Start,-NOTE%3A%20The%20Docker and save. 
8. After save - check - no error after check? - hit the up button and your docker service should be on now ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/2e3b1340-c964-4a42-bf88-1575d1572e62)
9. This how it looks like when your docker service is on ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/6a7dce52-d8b1-4d66-b710-bd791bfda39a)
10. This is how your docker storage looks like - **JUST LET IT BE, DO NOT MODIFY** ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/d2b9a0b7-5df9-4f9a-bcc9-7286740435a5) 
11. The "jdownloader" folder will be generate based on docker files compose. ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/b5ccfa6d-5cdb-445c-bc46-452a3aaa4e11)
12. In order to access the "output" folder, You need to create shared folder in omv - ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/10be4140-78ed-41a3-869c-7bbf6f9668eb)
13. Setup share in SMB to enable windows to discover the "output" folder - ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/cc607f0d-a986-4828-bd30-c0bded66bdb4)
14. Enjoy. ![image](https://github.com/khewweifeng/OMV6-DOCKER/assets/54496743/ee67cc9c-3478-4b3d-b9bc-6e325189f7ef)


