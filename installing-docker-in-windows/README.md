# Instructions

Open command line as administrator

Navigate to your batch file folder

Execute them one by one in this order:

hyperv.bat

container.bat

currentversion.bat

Do not reboot if prompted

Now download and run Docker Windows setup

Once finished -> Restart



Docker will now start. It may raise error though which it did in my case:

Hyper-V was unable to find a virtual switch with name "DockerNAT"

FIX HERE:

https://support.microsoft.com/en-us/help/3101106/you-cannot-create-a-hyper-v-virtual-switch-on-64-bit-versions-of-windo



Restart



Now you may check if your registry needs restoring. Mine reset after reboot automatically. But if it didn't ->

Run restore.bat