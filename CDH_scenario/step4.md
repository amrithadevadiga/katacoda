<br>Here we are looking in to all the configuration scripts like startscript & default scripts are in the directory named cdh5-cm-setup.
<br>
This directory contains all of the necessary files pre-created for standard services, including startscript, and appjob. 
You may change the name of this directory if desired.<br>

Execute the below command to list the all Files in cdh5-cm-setup directory <br>
`cd cdh5-cm-setup`{{execute}}<br>

<b>setup_cluster.py</b> script is responsible for setting up CDH Cluster <br>
<b>add_remove_node.py</b>  scripts is responsible for scaling up/down the nodes in CDH cluster<br>
<b>Enable_Kerberos.py</b> script enable Kerberos in CDH cluster<br>
<br>

Let's Look in to Startscript<br>
`cat startscript`{{execute}}

