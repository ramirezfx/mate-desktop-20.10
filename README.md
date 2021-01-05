# If you want to use the pre-build image do this:

`git clone https://github.com/ramirezfx/mate-desktop-20.10.git`

`cd mate-desktop-20.10`

`docker-compose up -d`

You have 2 methods to access the desktop

1) Download the latest NX-Client from https://www.nomachine.com/download/
Connect to the machine with the IP of the server and use this credentials
Username:mate
Password:mate
Once you are loged-in you can create a new user with su-rights and delete the default mate-user

2) Install x2go-client and connect to the machine via port 2222 and with this credentials:
Username:mate
Password:mate
Once you are loged-in you can create a new user with su-rights and delete the default mate-user

# If you want to build your own image do this:

`git clone https://github.com/ramirezfx/mate-desktop-20.10.git`

`cd mate-desktop-20.10`

Build the image:

`docker build -t myimage:latest .`

edit the file docker-compose.yml and change the values for USER and PASSWORD and the image

Start the container:

`docker-compose up -d`

You have 2 methods to access the desktop

1) Download the latest NX-Client from https://www.nomachine.com/download/
Connect to the machine with the IP of the server and use this credentials you entered in docker-compose.yml

2) Install x2go-client and connect to the machine via port 2222 and with this credentials you entered in docker-compose.yml
Once you are loged-in you can create a new user with su-rights and delete the default mate-user
