
## Jenkins Introduction:
Jenkins is a free and open-source automation server. It helps in automate the parts of software development related to building, testing and deploying, facilating cotinuous integration and continuos delivery.

## History :-
1. Original name of Jenkins in 2004 - Hudson. 
2. Creator of Jenkins - Kohsuke Kawaguchi (written in JAVA).
3. During November 2010, aften the acquition of Sun Microsystems by Oracle, an issue arose in the Hudson community with respect to the infrastructure used.
4. After a discussion, a new project initialise on 2nd Feb, 2011 - Jenkins
5. In 2011, creator Kohsuke Kawaguchi received O'Reilly Open source Award for his work on the project Hudson/ Jenkins.
6. On April 20,2016 version 2 was released with the pipeline plugth integration/enabled by default. The plugin allows for waiting build Instructions way a domain specific language on Apache groovy.

Jenkins is replaced Hudson Since February 8, 2017 in eclipse.

## Features:- 
* Continuous Integration and Continuous Delivery
* Easy installation. 
* Plugins (In today's would, there are many tools throughehich we can use plugins to integrate with Jenkins)
* Extensible (Anyone can integrate jenkins with the plugin architecture)
* Easy Configuration (easily setup and configured via its web Interface and which includes error checks and bult-in-help.
* Distributed (Jenkins can easily distributed across multiple machines, helping drive builds, tests and deployment across multiple platforms faster. Master-Slave architecture helps to reduce load)

## Sofware Development Life Cycle (SDLC)
* Analysis (clients Requirement)
* Design (future entire architecture 
* Implementation (write coding) 
* Testing (Tester team tells to developer about faulty things/issues. After iteration, tester team again test it)
* Deployment (Software run and then release for end users)
* Maintainance (Maintain the server)

## Feasibility Studies:
- Economic
- Legal
- Operation Feasibility
- Technical Possibility
- Schedule

## Installation of Jenkins by following the below document:
https://phoenixnap.com/kb/install-jenkins-ubuntu

sudo apt update</br>
sudo apt install openjdk-11-jdk -y</br>
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null</br>

echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null</br>

sudo apt update</br>
sudo apt install jenkins -y</br>
sudo systemctl status jenkins</br>
sudo systemctl enable --now jenkins</br>
sudo ufw allow 8080</br>
sudo ufw status</br>
sudo ufw enable</br>

## Open a web browser, and navigate to your server' IP address. Use the following syntax:
http://ip_address_or_domain:8080
       or
http://localhost:8080

* Unlocking Jenkins after installation.
A page opens prompting you to Unlock Jenkins. Obtain the required administrator password in the next step.

* Obtain the default Jenkins unlock password by opening the terminal and running the following command:
sudo cat /var/lib/jenkins/secrets/initialAdminPassword</br>
Obtaining the Jenkins administrator password.

* The system returns an alphanumeric code. Enter that code in the Administrator password field and click Continue.

* The setup prompts to either Install suggested plugins or Select plugins to install. It’s fine to simply install the suggested plugins.
Customizing Jenkins plugins after installation.</br>
You can always install more plugins later. The system continues the initial Jenkins setup.

* The next step is the Create First Admin User. Enter the credentials you want to use for your Jenkins administrator, then click Save and Continue.
Creating the first admin user in Jenkins./br>

* After this, you should set up the Instance Configuration. This is the preferred network address for this Jenkins installation. Confirm the address you want to use for your server. This is most likely the same address you used to get to this configuration page.
Configure the Jenkins instance.</br>
Once you specify the Jenkins URL, click Save and Finish.

* You should see a page that says Jenkins is ready! Click Start using Jenkins to open the Jenkins dashboard.
Complete Jenkins configuration on Ubuntu.

