# How to Install Ubuntu-18.04-on-M1 macs(VM)

# Step 1
Install VMware fusion for apple silicon 

https://blogs.vmware.com/teamfusion/2021/09/fusion-for-m1-public-tech-preview-now-available.html

<img width="1440" alt="Screenshot 2021-12-16 at 10 17 48 PM" src="https://user-images.githubusercontent.com/34735804/146413875-e24c0890-a26b-4dc5-90ec-ee5a456e0c00.png">
You would need to create an account then click on download (VMware-Fusion-e.x.p-18656771_arm64.dmg)

# Step 2
Install Ubuntu 18.04.06 live server for 64-bit ARM

https://cdimage.ubuntu.com/ubuntu-server/bionic/daily-live/current/

<img width="1440" alt="Screenshot 2021-12-16 at 10 23 31 PM" src="https://user-images.githubusercontent.com/34735804/146414580-431c16ed-d12c-43e5-bacb-58d976d75953.png">

# Step 3
Open VMware Fusion Tech Preview   
and drop the downloaded Ubuntu(bionic-live-server-arm64.iso) file   
and save it   
Now the VM starts

https://user-images.githubusercontent.com/34735804/146416021-023882fe-26f5-4e27-9058-affaea8c6a8a.mov

# Step 4
Click on virtual machine-> Shutdown    
then again click on virtual machine-> Settings

https://user-images.githubusercontent.com/34735804/146416653-ffabe510-deed-47b6-9b91-f00cf9bcfd91.mov

# Step 5
Here we are going to increase the hard drive space or SSD space for the vm    
Option 1 

Using VM through External HDD or SSD
       
          Add Device
          Click on New Hard Drive--> Add
          Adjust the Disk Size (Recommended 200 Gb)
          Click on File name---> Save as
          Change the Directory to that particular External HDD or SDD and save
          Click on apply
          Move back to settings by clicking on "Show all"
          Click on "Hard Drive" (not Hard Drive 2)
          Click on Remove Hard Drive
          
  https://user-images.githubusercontent.com/34735804/146422272-609a5d1c-ae2f-42df-bc4b-e7c3fad417da.mov

        

Option 2

Using VM through Mac SSD (Ask your mentor about how much space required for the VM.   BEFORE PROCEEDING)
               
          Click on "Hard Drive"
          Adjust the Disk Size (Ask your mentor)(tell him/her about your mac storage)
          Click on apply
               
# Step 6
Start the VM

https://user-images.githubusercontent.com/34735804/146423745-14b5d7c8-b97a-45ff-a705-eacbff4379e7.mov

Follow the installation process

# Don't update the software (In the process it might ask you to do so)
You are free to use any name for username and server name 

https://user-images.githubusercontent.com/34735804/146424801-ff9e9594-001a-4a5d-ad70-2f17e0adbf42.mov

https://user-images.githubusercontent.com/34735804/146425291-b4b6d1a3-1b9a-4ba2-b526-77f16cfa5ac7.mov

Wait for few mins

# Step 7
When you see this 

<img width="1440" alt="Screenshot 2021-12-16 at 11 37 04 PM" src="https://user-images.githubusercontent.com/34735804/146425564-6bc77589-60ad-4bae-a781-0b408aa3f518.png">

Just Press return


You will see ubuntu starts again

Enter your Username and Password

https://user-images.githubusercontent.com/34735804/146425857-9089fd83-1a75-497e-8967-308073305f71.mov

# Step 8
Use the command given one by one (So we can convert Ubuntu server to Ubuntu desktop (GUI))
    
         $ sudo apt install tasksel
         $ sudo tasksel install ubuntu-desktop
     
https://user-images.githubusercontent.com/34735804/146426735-0c3019cf-2499-486e-a71c-e085a7965305.mov

This takes time 

After this is installed 100%    
Use this command 

         $ sudo reboot
                     
https://user-images.githubusercontent.com/34735804/146428248-6acb3cb0-de4c-49b4-abad-84911a6839fa.mov

# Don't update to 20.04 But you need to do some updates(see the video)

https://user-images.githubusercontent.com/34735804/146429332-85b70aef-1ee2-46c1-b448-abf0a54a8c10.mov

But see the video below and do those updates

https://user-images.githubusercontent.com/34735804/146429645-68abd9a1-c69d-4120-b116-6d2a2ff2c0f3.mov

Now Ubuntu(arm64) running on m1 macs 

# Now Reboot the VM

If it shows "Start PXE over IPV4"    
Do this    
Shutdown the VM    
Open Settings    
Click on Add device->Network Adapter->Add    
Move back to settings (by clicking ‘show all’)        
Click on ‘Network Adapter’-> Advanced Options->Remove Network Adapter (I faced a issue where it only boots via network every time you start the vm)   
(This solves that)

Now Start Again 

If it still occur just    
disconnect the network adapter   
and turn it on after you see sign in window   


                     
                     
                     
                     




               
               
          
          
          
      
