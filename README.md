How to install Jenkins and a Pipeline
=====================================

This repo contains step-by-step instructions to install [Jenkins](https://jenkins.io) and a sample [Pipeline](https://www.jenkins.io/doc/book/pipeline/) for CI/CD (Continuous Integration and Continuous Delivery/Deployment).

🔧 Install the Jenkins server
------------------------------
* Execute for Docker: `docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk11`
* Execute for Linux Snaps: `sudo snap install --classic jenkins`
* Otherwise, download and install it from: https://jenkins.io/download (available for Arch Linux, FreeBSD, Gentoo, macOS, OpenBSD, OpenIndiana Hipster, openSUSE, Red Hat/Fedora/Alma/Rocky/CentOS, Ubuntu/Debian, Windows)

NOTE: Pipelines are supported in Jenkins version 2.337 or newer.

💻 Browse to your new Jenkins server
-------------------------------------
Launch your Web browser and enter the URL: **http://HOSTNAME:8080** (replace HOSTNAME by the computer name where Jenkins has been installed).

🔓 Unlock Jenkins
-----------------
1. Execute `sudo cat /PATH/TO/initialAdminPassword` (replace /PATH/TO) to view the initial password saved by Jenkins during the installation.
2. Enter the initial password to unlock Jenkins.

📌 Install necessary Plugins
-----------------------------
1. Click on **'Select plugins to install'**
2. Add these plugins: **'Build Name and Description Setter'**
3. Click **Install** and wait until the installation has finished.

🧙‍♂️ Create the Admin Account
---------------------------
1. Enter the username, password (twice), and the full name.
2. Afterward, enter your Jenkins URL and log in.
     
📝 Create a Pipeline
---------------------
1. In the dashboard click on: **+ Create element** (on left side).
2. Enter a job name (e.g. "sample-pipeline") and select **Pipeline**, then press the OK button.
3. The job configuration is displayed now - scroll down and select the **Pipeline script**.
4. As script enter the content of the **Jenkinsfile** (attached to this repository).
5. Click the **Save** button.
     
▶️ Start the Pipeline Job
-------------------------
1. Click on **Dashboard** (on left side).
2. In your job list press the green **Play** button (on right side).
3. The **Stage View** visualizes the whole build process in a neat table.
  
🏆 Congratulations
-------------------
* You're done. Welcome to the Jenkins ecosystem! More background information can be found here:
* Jenkins **Homepage** at: https://www.jenkins.io
* Jenkins **User Documentation** at: https://www.jenkins.io/doc
* Jenkins **Handbook** at: https://www.jenkins.io/doc/book

🚀 What's Next?
----------------
* Discover **1800+ plugins** to extend your Jenkins installation at: https://plugins.jenkins.io
* Install the **Jenkins app** on your smartphone to trigger builds anytime anywhere. It's available for free at: https://play.google.com/store/apps/details?id=com.mobilabsolutions.jenkins.app
* Add more machines for a **distributed build environment**. More information at: https://www.jenkins.io/doc/book/using/using-agents
* Add **more Pipelines** using GitHub projects with a Jenkinsfile. The following table lists some:

| GitHub Project | URL                                         | Path to Jenkinsfile |
|----------------|---------------------------------------------|---------------------|
| base256        | https://github.com/fleschutz/base256unicode | Jenkinsfile         |
| CWTS           | https://github.com/fleschutz/CWTS           | Jenkinsfile         |
| PowerShell     | https://github.com/fleschutz/PowerShell     | data/Jenkinsfile    |


📧 Feedback
------------
Anything missing or is incorrect? Don't be shy, just send your email feedback to: markus.fleschutz [at] gmail.com

🤝 License & Copyright
-----------------------
This open source project is licensed under the CC0 license. All trademarks are the property of their respective owners.
