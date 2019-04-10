Let's install App workbench version 3.4 

Skills needed:
<ul>
  <li>Ability to install applications manually</li>
  <li>Familiarity with shell and python scripting</li>
  <li>Linux admin skills</li>
</ul>
Note: Install java, Spark, Webssh on all nodes

1. Download scripts from 

`wget https://files.pythonhosted.org/packages/b0/20/a95abd315193ac23a16dbe04ba582dc8d7372d55a1730846a7d25136bdb5/bdworkbench-3.4.tar.gz`{{execute}}

2.Extract the bdworkbench tar file by executing this command
`tar -xvf bdworkbench-3.4.tar.gz`{{execute}}

3.Change the directory to bdworkbench
`cd bdworkbench-3.4`{{execute}}

4.Execute the command sudo python setup.py install
`sudo python setup.py install`{{execute}}

5.To install app workbench dependencies using yum
`yum install -y python-setuptools`{{execute}}

6.To check the installed app work bench version
`bdwb --version`{{execute}}

7.The workbench has inline help. Try the following
`bdwd` {{execute}}

`help`{{execute}}

`help catalog`{{execute}}

`help catalog new`{{execute}}

`Exit`{{execute}}



<b>App Catalog – Node, Role, and Service</b>

BlueData catalog allows users to map a deployment strategy in a json file, and use this json as a guide while stating the cluster. Same Docker image can be used in multiple strategies. 
<br>Catalog file includes:
<br>
<br>Node - A running docker container instance. A cluster can have several nodes, spread on several physical hosts
<br>
<br>Role - A type of a container.  Example: worker, master, edge, etc. A cluster can have zero or more containers of each role after deployment
<br>
<br>Service - A list of all possible services registered for a given cluster. Example: CM Server, CM Agent.NameNode, DataNode, Yarn RM, NodeManager, Hive Thrift Sever, 
<br>
<br>Role to Service mapping -  Defining the association of what list of services run on which role. Example: NameNode and Yarn RM runs on master. DataNode and NodeManager runs on worker.


