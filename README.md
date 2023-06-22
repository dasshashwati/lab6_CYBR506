# lab6_CYBR506: How to use a RADIUS server for authentication
image name as freeradius1
Container name as  freeradius23
Create a Docker Container for RADIUS --
 place the command on powershell docker build -t freeradius1 .
After the image created then put as command  docker run -d --name freeradius23 -p 1812:1812/udp -p 1813:1813/udp freeradius1
To see the IP address ---docker inspect freeradius1
the modified RADIUS configuration files are stored in a directory named raddb that resides under Freeradius
Changes to the RADIUS Config Files :update the username and password 
     check on web :http://127.0.0.1:5000
      User: mou    Cleartext-Password := "password1"
will see the msg "Welcome mou"
