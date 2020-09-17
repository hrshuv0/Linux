




# installing the Default JRE/JDK

To install this version, first update the package index:

    sudo apt update
    
Next, check if Java is already installed:

    java -version
    
If Java is not currently installed, you’ll see the following output:
## Output

    Command 'java' not found, but can be installed with:

    sudo apt install default-jre              # version 2:1.11-72, or
    sudo apt install openjdk-11-jre-headless  # version 11.0.7+10-3ubuntu1
    sudo apt install openjdk-13-jre-headless  # version 13.0.3+3-1ubuntu2
    sudo apt install openjdk-14-jre-headless  # version 14.0.1+7-1ubuntu1
    sudo apt install openjdk-8-jre-headless   # version 8u252-b09-1ubuntu1


install the JRE from OpenJDK 11:

    sudo apt install default-jre
    
    
Verify the installation with:


    java -version
    
    

You’ll see the following output:
## Output


    openjdk version "11.0.7" 2020-04-14
    OpenJDK Runtime Environment (build 11.0.7+10-post-Ubuntu-3ubuntu1)
    OpenJDK 64-Bit Server VM (build 11.0.7+10-post-Ubuntu-3ubuntu1, mixed mode, sharing)
    
    
    
    
You may need the Java Development Kit (JDK) in addition to the JRE in order to compile and run some specific Java-based software. To install the JDK, execute the following command, which will also install the JRE:


    
    sudo apt install default-jdk
    
    
Verify that the JDK is installed by checking the version of javac, the Java compiler:


    javac -version
    
    
You’ll see the following output:
## Output

    javac 11.0.7
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    ###################
    
    
    
    
    
    
    
    
    
    
    














copy the file to "/opt" folder

    sudo mv spring-tool-suite-4-4.8.0.RELEASE-e4.17.0-linux.gtk.x86_64.tar.gz /opt/


go to opt folder

    cd /opt/

make sure move has done successfully

    ls


unzip file

    sudo tar -xvf spring-tool-suite-4-4.8.0.RELEASE-e4.17.0-linux.gtk.x86_64.tar.gz
    
    
make sure extract done sucessfully

ls

## output
for me:

    google
    spring-tool-suite-4-4.8.0.RELEASE-e4.17.0-linux.gtk.x86_64.tar.gz
    sts-4.8.0.RELEASE


go extract folder
    cd sts-4.8.0.RELEASE


# Make Desktop entry for STS

opn STS.desktop file
    sudo nano /usr/share/applications/STS.desktop


    [Desktop Entry]
    Name=SpringSource Tool Suite
    Comment=SpringSource Tool Suite
    Exec=/opt/sts-4.8.0.RELEASE/SpringToolSuite4
    Icon=/opt/sts-4.8.0.RELEASE/icon.xpm
    StartupNotify=true
    Terminal=false
    Type=Application
    Categories=Development;IDE;Java;


after write these line

press:

    ctrl+x
    
    y
    
    enter
    
    


