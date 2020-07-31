# Upload Release To GitHub

Move rom.zip to git device tree repo folder.

    sudo snap install hub --classic
    cp -v rom.zip ../../../../device/oppo/CPH1859
    hub release create -a rom.zip -m "Release Message" v1

# Upload Release To SourceForge

    scp rom.zip username@frs.sourceforge.net:home/frs/project/realme1/RomFolder

# Upload Release To Bashupload 

    curl https://bashupload.com/rom.zip --data-binary @rom.zip
    
File is stored for a week only.

# Upload Release To Transfer.sh

    curl --upload-file ./rom.zip https://transfer.sh/rom.zip

File is stored for two weeks.
