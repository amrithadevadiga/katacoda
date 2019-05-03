We need to add additional configuration files, We already have a reference configuration files, To add them follow the below steps

Remove the existing set-up folder from the HDP folder
rm -rf ambari-26-setup.zip{execute}}

Add the reference file using the below command from stored location(Due to space constraint in Katacoda we have uploaded the required files into dropbox)
wget https://www.dropbox.com/s/0bops5b1ai4yp1k/ambari-26-setup.zip{{execute}} 
yum install unzip -y{{execute}}

Unzip the file
unzip ambari-26-setup.zip{execute}}

Check files under appconfig directory
ls ambari-26-setup.zip{execute}}
