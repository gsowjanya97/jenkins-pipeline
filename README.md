# Jenkins Pipeline to Build Docker Image
#### Run the following commands on Azure VM before running the pipeline


``` shell
sudo chmod 777 <jenkins workspace path>
sudo usermod -a -G docker jenkins
sudo systemctl restart jenkins
```