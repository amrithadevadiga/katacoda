Lets build a .wb file  <br>
<br>
<b>.wb</b> file contains a series of App Workbench commands that control the creation of the Catalog Image<br>
Please review the link before proceeding for wb file: [Link](http://docs.bluedata.com/awb34_applications-with-multiple-images)
<br>
<br>
Move to HDP directory:<br>
`cd ~/Source/HDP`{{execute}}<br>
For your reference, we have already created a ready .wb file in the ~/test directory. We will copy that file into the HDP directory using the following command:
<br>
`cp ~/test/hdp26-ambari26.wb ~/Source/HDP`{{execute}}

To view the content of .wb file, execute the following command:<br>
`cat ~/Source/HDP/hdp26-ambari26.wb`{{execute}}

<br><strong>hdp26-ambari26.wb file contain following section</strong>
<br>
<br><b>Section 1:</b> <br>
<br><b>The below line will Set the organization name.</b>
<br>builder organization --name BlueData
<br>
<br><b>The below line will load the Metadata JSON file and set up files</b>
<br>catalog load --filepath hdp26-ambari26.json
<br>appconfig package --dir ambari-26-setup
<br>
<br><b>The below line will add the logo file to the image</b>
<br>logo file --filepath Logo_HortonWorks.png

<br><b>Section 2:</b> <br>
<br><b>Below section of the .wb file pulls all of the pieces together and builds the .bin file.</b>
<br>image build --basedir image/centos --image-repotag bluedata/hdp26-ambari26-7x-macys:1.0
<br>image package --image-repotag bluedata/hdp26-ambari26-7x-macys:1.0 --os centos7
<br>catalog save --filepath staging/hdp26ambari26-centos.json --force
<br>sources package
<br>catalog package

<br>When our image is ready to deploy in the EPIC Application Catalog, we need to include a picture that represents the image. For your reference, we have already created a .png file for your use.
<br>`cp ~/test/Logo_HortonWorks.png ~/Source/HDP`{{execute}}<br>
<br><b>Logo.png file</b> includes a logo file (400px x 200px .png) to visually identify each application in the App Store
