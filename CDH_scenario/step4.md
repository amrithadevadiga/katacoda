<br>Here we are looking in to all the configuration scripts like startscript & default scripts are in the directory named cdh5-cm-setup.
<br>
This directory contains all of the necessary files pre-created for standard services, including startscript, and appjob. 
You may change the name of this directory if desired.<br>

Execute the below command to list the all Files in cdh5-cm-setup directory <br>
`ls cdh5-cm-setup`{{execute}}<br>

<b>setup_cluster.py</b> script is responsible for setting up CDH Cluster <br>
<br><b>add_remove_node.py</b>  scripts is responsible for scaling up/down the nodes in CDH cluster<br>
<br><b>Enable_Kerberos.py</b> script enable Kerberos in CDH cluster<br>
<br><b>Macros.sh</b> contains all the built in macros of BlueData that would be executed during image creation.
<br>
<br><b>Logging.sh</b> provides the logging facilities for a catalog configuration bundle. 
<br>
<br><b>Utils.sh</b> contains utility functions defined which provides information on docker id, cpu share, memory status and fqdn of the current container.<br>
<br><b>appjob</b> provides the information on the type of job to be launched and we can also add application specific jobs.<br>
<br>

Let's Look in to Startscript<br>
`cat startscript`{{execute}}
<br>
<br>Start script will execute in each and every host when all host get created 
<br>After creating the hosts cloudera manager and agent gets register in each host
<br>Then Mysql database gets deployed in cmserver role and also cloudera database will be created.
<br>After that main setup script gets executed
<br>The main script in files contain code for Cluster creation, Activating licence ,Deploying zookeeper, hdfs and other services


