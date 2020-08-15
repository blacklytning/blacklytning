# Create A New User

Add User Command
    
    adduser zenith
  
Grant sudo permission.

    usermod -aG sudo zenith

Switch to the user
  
    su - zenith
   
Update all packages

    sudo apt update && sudo apt upgrade -y

Set up build env

    cd ~ && sudo apt install git -y && git clone https://github.com/akhilnarang/scripts && cd scripts && sudo bash setup/android_build_env.sh
