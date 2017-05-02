# UnauthorizedMongoDB
You should use ZMAP to scan the IPs which open mongoDB port(27017) and save the IPs in a file, here I use the file named "output.txt" or You can use whatever.

check login for unauthorized mongoDB

#Step1 scan the IPs open port 27017

zmap xxx.xx.xxx.0/24 -p 27017 -o ip.txt

#Step2 check the unauthorized Mongodb servers

python mongodb_check.py ip.txt
