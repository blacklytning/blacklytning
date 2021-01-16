# Upload Release To GitHub
  
  Keep file in repo.
  
    sudo snap install hub --classic
    hub release create -a rom.zip -m "Release Message" v1

# Upload Release To SourceForge

    scp rom.zip username@frs.sourceforge.net:home/frs/project/realme1/RomFolder

# Upload Release To Bashupload 

    curl https://bashupload.com/rom.zip --data-binary @rom.zip
    
File is stored for a week only.

# Upload Release To Transfer.sh

    curl --upload-file ./rom.zip https://transfer.sh/rom.zip

File is stored for two weeks.

# Upload Release To 0x0.st

    curl -F'file=@rom.zip' http://0x0.st
   
File size limit 512MB. Stored for a month.
