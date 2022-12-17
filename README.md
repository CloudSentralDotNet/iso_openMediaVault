Manual available at;

https://github.com/CloudSentralDotNet/iso_openMediaVault/blob/master/Manual-OpenMediaVault-OMV5.pdf


Download selected ISOs via the links shown below ( or from https://github.com/CloudSentralDotNet/iso_openMediaVault/releases/ ) :
  
* https://github.com/CloudSentralDotNet/iso_openMediaVault/releases/download/v5.5.5.11/openmediavault_5.5.11-amd64.iso
* https://github.com/CloudSentralDotNet/iso_openMediaVault/releases/download/v4.1.22/openmediavault_4.1.22-amd64.iso 


Burning ISO / IMG to a USB Drive using 'dd'

* Insert a new USB drive but do not mount it.
* Check drive designation by running 'sudo lsblk' in a console.
* Run 'sudo dd bs=4M if=/path/to/pfsense.iso of=/dev/sdX status=progress && sync' 
  Replace sdX with your USB drive designation, for example: sdc (be very careful here!).
* The sync part is important, do not omit it!

After dd command finishes, your drive is ready.
