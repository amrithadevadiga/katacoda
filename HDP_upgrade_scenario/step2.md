For upgrading the image, we will be using a bin file of the existing image already developed. Let us download a .bin file to the directory we have created in the earlier step. 
<br>
Before that, let us install wget package. For doing so, execute the following command
<br>
`yum install wget -y`{{execute}}<br>
<br>
Now, navigate to the Source directory.
<br>
`cd ~/Source`{{execute}}
<br>
<br>
Download the bin file by executing the following command.
<br>
`wget https://www.dropbox.com/s/xyv64z1xt9l6lw7/bdcatalog-centos7-bluedata-cdh514_centos7x-1.7.tar`{{execute}}
<br><br>
Extract the content of the tar file by executing the following command
<br>`tar xvf bdcatalog-centos7-bluedata-hdp25-ambari-3.3.bin.tar`{{execute}}
<br><br>
Now, Make the .bin file executable by executing the following command<br>
`chmod +x bdcatalog-centos7-bluedata-hdp25-ambari-3.3.bin`{{execute}}

