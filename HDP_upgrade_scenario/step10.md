Let's see what you have built.
The newly built application package (or bundle) is saved in the deliverables directory. 
<br>`cd deliverables`{{execute}}
<br>`ls `{{execute}}

Congratulations you have successfully upgraded the HDP image.

To make the new image appear in App Store.
Copy the bin file to /srv/bluedata/catalog using the following commad
<br>`cp bdcatalog-centos7-bluedata-hdp26-ambari26-1.0.bin /srv/bluedata/catalog`

Make it an executable using the below command
<br>`chmod +x bdcatalog-centos7-bluedata-hdp26-ambari26-1.0.bin`

Go to App Store in the EPIC GUI and click on <b>Refresh </b>button to bring the image in to App Store.

Once the image appears on the App Store click on <b>Install </b> button to install the image.

![alt text](https://dzf8vqv24eqhg.cloudfront.net/userfiles/7467/9720/ckfinder/images/AppWorkbench/Walkthrough/example_3.jpg)

