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

      
         

   
    
