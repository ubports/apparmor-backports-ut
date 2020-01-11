## AppArmor backports for Ubuntu Touch
This repository contains kernel backports for the AppArmor 3 support which is required in Ubuntu Touch. They are conveniently prepared as a replacement folder for security/apparmor.

### Applying the patch
* Delete the folder apparmor in the security folder of your kernel entirely
* Unpack the contents of the archive into the security folder as a replacement
* Try to compile the kernel. Ideally they will work without further actions
* In case of compile errors, which can happen due to Google or the vendor having messed up the kernel interfaces, you need to fix them either in the kernel or in the apparmor folder. Normally it is easier to do in the apparmor folder, since when you modify the kernel interface it can affect a ton of files.


