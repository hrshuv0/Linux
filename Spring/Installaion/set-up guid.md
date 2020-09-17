






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
    
    


