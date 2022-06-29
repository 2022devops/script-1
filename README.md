# script-1
training to script
#!/bin/bash




echo "please enter the username"
read USER_NAME

grep ${USER_NAME} /etc/passwd

if
  [$? -eg 0 ]

then
echo "USer ${USER_NAME} exists on this system"
else
echo "User ${USER_NAME} does not exists on this system" 
