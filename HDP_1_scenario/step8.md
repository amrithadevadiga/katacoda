We need to add additional configuration files, Lets see the files in below steps

Check files under appconfig directory
`ls ambari-24-setup`{{execute}}

Make sure you see following files unders appconfig folder:<br>

<b>Startscript</b> is a script file which contains code to start all service(s).<br>
<br><b>appjob</b> provides the information on the type of job to be launched and we can also add application specific jobs.<br>
<br><b>Logging.sh</b> This provides the logging facilities for a catalog configuration bundle.<br> 
<br><b>Utils.sh</b> contains utility functions defined which provides information on docker id, cpu share, memory status and fqdn of the current container.<br>



