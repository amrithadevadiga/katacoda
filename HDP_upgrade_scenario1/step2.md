For upgrading the image, we will be using a bin file of the existing image already developed. Let us download a .bin file to the directory we have created in the earlier step. 
<br>
Before that, let us install wget package. For doing so, execute the following command
<br>
`yum install wget -y`{{execute}}<br>
<br>
Now, Copy the bin file from into Source Directory.
<br>
`wget https://www.dropbox.com/s/2mh0pzsq1092xr8/bdcatalog-centos7-bluedata-hdp25-ambari-3.3.bin.tar.gz`{{execute}}<br>
<br>`tar xvf bdcatalog-centos7-bluedata-hdp25-ambari-3.3.bin.tar.gz`{{execute}}
<br>
Copy the bin file to source directory
<br>
`cp bdcatalog-centos7-bluedata-hdp25-ambari-3.3.bin /root/Source/`{{execute}}
<br>
<br>
Now, Remove all folders which are pre-installed to save the space. <br>
<br>`rm -rf $(ls | grep -v Source | grep -v test)`{{execute}}
<br>
Now, navigate to the Source directory.
<br>
`cd ~/Source`{{execute}}
<br>
<br>
Now, Make the .bin file executable by executing the following command<br>
`chmod +x bdcatalog-centos7-bluedata-hdp25-ambari-3.3.bin`{{execute}}

