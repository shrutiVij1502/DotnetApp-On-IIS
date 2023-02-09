### Step 1 - Launch one windows EC2 instance and Enable the IIS  

Reference - https://www.youtube.com/watch?v=qdFPS1ywlho&t=707s

### Step 2 - Install the IIS hosting Engine and dotnet 

IIS installation File - 

https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-aspnetcore-7.0.2-windows-hosting-bundle-installer

Dotnet installation fille

https://dotnet.microsoft.com/en-us/download/dotnet/7.0


![MicrosoftTeams-image](https://user-images.githubusercontent.com/67600604/216295527-60125eb9-9551-406c-bb4c-26c81b91400f.png)


### Step 3 - Create site and give the whole publish path of the path as the destination.

Put the path where the .exe and related files are located
Create a blankApp on Visual studio and build then Start the Application, then publish the site and then copy the publish folder's path and then paste the whole folder into the Window EC2 and mention the same ec2 folder path in the Destination of the IIS site creation

![MicrosoftTeams-image](https://user-images.githubusercontent.com/67600604/216296196-26a4b997-bd80-48e5-9d66-31b50d1f5208.png)

![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/67600604/216296261-567badfc-be27-46c6-ba97-53b33e8402db.png)

### Step 4 - Create the Site in IIS and write click on it.

![MicrosoftTeams-image (2)](https://user-images.githubusercontent.com/67600604/216296320-e52f34d6-4df0-48fe-8665-aa20b40096c5.png)

then type "Users" and check names , after that provide the permission to the Users profile.

### Step 5 - Hit the website.

![MicrosoftTeams-image (3)](https://user-images.githubusercontent.com/67600604/216296399-ce0d358e-352d-4736-917c-5abd74e67f21.png)

### Step 6 - The site that is hosted on the port other than 80 would not be accessible through the outer Internet , for this , we have to manually add the inbound rule in the windows system

https://learn.microsoft.com/en-us/archive/blogs/mandi/how-to-create-a-windows-firewall-inbound-rule
