If you want to use the pre-build image do this:

git clone https://github.com/ramirezfx/mate-desktop-20.10.git
cd mate-desktop-20.10
docker-compose up -d

You have 2 methods to access the desktop
1) Download the latest NX-Client from https://www.nomachine.com/download/
Connect to the machine with the IP of the server and use this credentials
Username:mate
Password:mate
Once you are loged-in you can create a new user with su-rights and delete the default mate-user

If you want to build your own image do this:

git clone https://github.com/ramirezfx/mate-desktop-20.10.git
cd mate-desktop-20.10

Build the image:
docker build -t myimage:latest .
