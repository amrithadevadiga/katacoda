
Let's build a CentOS 7 base image.

Create a directory for base images and navigate to it

`mkdir -p ~/src/base_images.`{{execute}}

`cd ~/src/base_images.`{{execute}}

You are in the base image directory.

Please review the link before proceeding: [Link](http://docs.bluedata.com/awb34_bdwb-shell-commands)

Retrieve the BlueData base image for CentOS 7 using bdwb command

`bdwb --baseimg centos7`{{execute}}

A CentOS 7 directory will be created in the current directory. Navigate to it.

`cd centos7`{{execute}}

To list the contents inside centos7 directory execute the below command

`ls -a`{{execute}}

Make sure the Build.sh, Makefile and Template are present. 

<b>Build.sh</b> is a file that contains a build script to build the centos7 image<br>
<br>
<b>Makefile</b> is a program building tool which runs on Unix or Linux<br>
<br>
<b>Template</b> is a directory that houses the Dockerfile.template and limits-90-nproc.conf files<br>

To add your organisation name to the build, run the following command:

Here we have used
Organization name as BlueData

`export BASE_IMG_ORGNAME='bluedata'`{{execute}}

To identify your build, you add a build version to image. To do so run the following command:

`export BASE_IMG_VERSION='1.0'`{{execute}}

By default, the upstream image source is centos:centos7

`export CENTOS7_UPSTREAM='centos:centos7'`{{execute}}

where <b>upstream</b> is the name of the upstream image source, such as artifactory.com/enterprise:centos7. The default upstream image source is centos:centos7.

Make the new centos7 image by executing the following command

`make centos7`{{execute}}


