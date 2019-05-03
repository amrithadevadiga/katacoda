We need to add additional configuration files under appconfig directory, We already have a reference configuration files, To add them follow the below steps

Remove the existing appconfig folder from the Spark folder
rm -rf appconfig{{execute}}

Add the appconfig reference file using the below command from stored location(Due to space constraint in Katacoda we have uploaded the required files into dropbox)
wget https://www.dropbox.com/s/f8cjkwzz6qdov0d/appconfig.zip{{execute}} 
yum install unzip -y{{execute}}

Unzip the file
unzip appconfig.zip{{execute}}

Check files under appconfig directory
ls appconfig{{execute}}
