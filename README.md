# Requires software
* [JDK] - JDK 1.8 (not JRE)
* Eclipse IDE
* Gradle
* Docker
* Lombok for Eclipse
* ConEmu
* AWS CLI
* SSH Client: PuTTy, CygWin w/ ssh, etc.
* SCP Clinet: WinScp


## JDK install
  - Download and install JDK from Oracle site
  
  https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
  - Make sure you choose JDK not JRE package
  - Once installation complete, to verify, open new Terminal/Command Prompt and check java version by typing "java -version". If it indicates JDK 1.8 then it is all set
  - If not, make sure JAVA_HOME is set properly
  
  For Mac/Linux: 
  
https://www.mkyong.com/java/how-to-set-java_home-environment-variable-on-mac-os-x/

  For Windows: 
  
https://docs.oracle.com/cd/E19182-01/820-7851/inst_cli_jdk_javahome_t/

## Eclipse IDE
  - Download and install Eclipse from here
  
  https://www.eclipse.org/downloads/
  - You can pick latest version of Eclipse

## Lombok Eclipse plugin
  - Lombok is Eclipse plugin to avoid boiler plates in Java code
  - Install Lombok and follow instruction from here
  
https://projectlombok.org/setup/eclipse

  - Once you install Lombok, you will need to restart Eclipse


## Gradle
  - Gradle is dependency management tools. It requires Java to be installed, thus make sure you have JDK install first
  - Install Gradle from here
  
https://gradle.org/install/#prerequisites
  - You can pick latest greatest version of Gradle
  - Make sure that gradle is in the path so it can be invoked from any where. Or you can setup GRADLE_HOME as well

## Docker
  - Install docker from official Docker site
  
https://docs.docker.com/install/
  - Choose docker agent based on your operating system (Mac/Linux/Windows)
  - Just pick stable release from Docker
  - Once installation is complete, go to Terminal/Command Prompt and type "docker --version" to verify
  
## ConEmu
  - ConEmu is handy terminal emulator for Windows (similar to PowerShell)
  - Install ConEmu from here
  
  https://conemu.github.io/

## AWS CLI
 - AWS CLI is command line interface tools which is needed in this training 
 - Please refer to AWS documentation below for installation

https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html

## PuTTy and PuttyGen
 - If you are using Windows, you will need both Putty and PuttyGen to connect to Linux instances
 - If you are using Mac/Linux, you can just use ssh
 - To download Putty, navigate below

https://www.putty.org/

 - To download PuttyGen, navigate below

https://www.puttygen.com/

## WinScp
https://winscp.net/eng/download.php


## Connecting to Linux instance
 - Make sure you have the pem key and store them in .ssh folder
 - If you are using Mac/Linux: 
     ssh ec2-user@[ip address]
- If you are using Windows:
     * Open up PuttyGen
     * Click Load and choose pem key that you have
     * You need to convert them to ppk file
     * Save private key
     * Open up Putty
     * In the hostname, type EC2 IP Address
     * In the Putty menu on left, choose SSH
     * Choose Auth
     * Click Browse
     * And select ppk file that you generated earlier with PuttyGen
     * Once you are login, for the user, type "ec2-user"
     
For detail information, you can refer here:
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/putty.html
