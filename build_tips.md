# Telephony Patches (Not Necessary)
      git clone https://github.com/AgentFabulous/vendor_mediatek_hardware_telephony-ext -b wip vendor/mediatek/hardware/telephony-ext
      git clone https://github.com/PeterCxy/vendor_mediatek_hardware_interfaces.git -b lineage-17.0 vendor/mediatek/hardware/interfaces
      git clone https://github.com/LineageOS/android_hardware_mediatek -b lineage-17.1 hardware/mediatek

# Install/Uninstall Patches
      sh device/oppo/CPH1859/patches/install.sh
      sh device/oppo/CPH1859/patches/uninstall.sh

# Android 10 Cache
      export USE_CCACHE=1 && export USE_CCACHE_EXEC=$(command -v ccache) && ccache -M 80G && export ANDROID_JACK_VM_ARGS="-Xmx15g -Dfile.encoding=UTF-8 -XX:+TieredCompilation"
Sets cache limit to 80GB replace 80 with smaller number if diskspace is low.   

# Clone Device Tree
      workingdir/device/brand/codename
      
# Clone Vendor Tree
      workindir/vendor/brand/codename     

# Start Build
This is different for each rom check their manifest.
      
      . build/envsetup.sh
      lunch customrom_codename-userdebug
      brunch codename
      
# Set up Repo Tool
      mkdir ~/bin
      PATH=~/bin:$PATH
      curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
      chmod a+x ~/bin/repo
      
# Establish Build Env
      sudo apt-get update && sudo apt-get upgrade
      sudo apt-get install android-tools-adb android-tools-fastboot git-core gnupg flex bison gperf build-essential zip curl zlib1g-dev gcc-multilib g++-multilib libc6-dev-i386 lib32ncurses5-dev x11proto-core-dev libx11-dev lib32z-dev libgl1-mesa-dev libxml2-utils xsltproc unzip python bc bison build-essential ccache curl flex g++-multilib gcc-multilib git gnupg gperf imagemagick lib32ncurses5-dev lib32readline6-dev lib32z1-dev liblz4-tool libncurses5-dev libsdl1.2-dev libssl-dev libwxgtk3.0-dev libxml2 libxml2-utils lzop pngcrush rsync schedtool squashfs-tools xsltproc zip zlib1g-dev 
      
# Set Up Git Config
      git config --global user.name "blacklytning"
      git config --global user.email "blacklytning@yandex.com"
     
# Sync Repo
Check ROM's manifest to sync repo
      
