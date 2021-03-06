To begin the application development, we will first need to create a directory called “Spark” or any directory name of your choice. This directory will house all the files and components necessary to create the application image. 

To create a directory, execute the following command:<br>
`mkdir ~/Spark`{{execute}}<br>

Navigate to your new source directory:<br>
`cd ~/Spark`{{execute}}<br>

Next, we need to create a skeleton file structure. To do so execute the following command:

`bdwb --init`{{execute}}

 <b>bdwb --init</b> command will setup all the base directories and files you need in order to develop any app image

 Execute the below command to list all the files and folders created by bdwb command:<br>
`ls -R`{{execute}}

Make sure that you see the following files or directories:
<br>appconfig/<br>
appjob  <br>
logging.sh  <br>
macros.sh  <br>
startscript  <br>
utils.sh<br>
image/

Above files are required for Spark Application Image development.<br>
<br>
Here <b>Startscript</b> is a script file which contains code to start all service(s). 
<br>
<br><b>Macros.sh</b> contains all the built in macros of BlueData that would be executed during image creation.
<br>
<br><b>Logging.sh</b> provides the logging facilities for a catalog configuration bundle. 
<br>
<br><b>Utils.sh</b> contains utility functions defined which provides information on docker id, cpu share, memory status and fqdn of the current container.<br>
<br><b>appjob</b> provides the information on the type of job to be launched and we can also add application specific jobs.<br>
<br>Now, we will create a folder called “centos” inside the empty image directory. Execute the following command to do so :
<br>`mkdir ~/Spark/image/centos`{{execute}}
