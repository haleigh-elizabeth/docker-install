# docker-install
##installing docker.io and openvas
---
* **Step 1:** Trouble shoot a project for hours, cry, then ask Codi why it won't work
* **Step 2:** Figure out it is because you don't actually have the real version of Ubuntu installed!
* **Step 3:** Make sure you have properly installed ubuntu
* **Step 4:** Run these comands
  *  <span style="color:blue">some install sudo apt-get text</span>
  * sudo apt-get install docker.io
  * press y to continue installing
  * sudo service docker start
* You have downloaded docker! 
* Type in status to see that your docker is running
* **Step 5:** Install the container (openvas)
  * sudo docker run -d -p443:443 --name openvas mikesplain/openvas
* This step will take about 5 mins to install
* Even after the "install" is done, the security functions of opencvas can take up to 20 mins to install
   * To check if the security functions are installed, check sescurity monitor and if your CPU useage is very high, it is still downloading
* **Step 6:** Run openvas
   * Open a web browser (I used firefox)
   * Type: https://localhost/
   * A security risk window will pop up but do not worry! We just dont have a signed certificate yet.
       * Click "advanced"
       * Click "accept risk and continue"
* **Step 7:** Login!
   * Username: admin
   * Password: admin
