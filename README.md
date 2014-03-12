This application is a browser based client for the impression_mark services. This web application uses the embedded tomcat approach to launch the server. For illustration visit the following link. 

	https://github.com/heroku/devcenter-embedded-tomcat
	
Pre Requisites
---------------

1) Impression Mark service should be running. Please refer the following given link for more details.
	
	https://github.com/iamon3/impression_mark
	
2) Apache Maven

3) Access to git


Project Set up
---------------

1) Clone this repository

  	git clone https://github.com/iamon3/impression_mark_webapp.git
  	
2) Go to the folder i.e. cloned repository

	$ cd {repository cloned path}/impression_mark_webapp

3) Build the project

	$ sudo mvn clean; sudo mvn package
	
This step will take some time as it will download all the required dependencies for compiling and running the web app.

4) Launch the application

	$ sudo sh target/bin/webapp
	
Done!  Your browser based client application is up and ready to serve the requests.

5)  Make sure that the impresion_mark service is up and running at port 9090. For details, refer pre requisite section. Open any browser and visit the URL.

	http://localhost:9090/hello
	
6) To stop the server on linux, on terminal where server is started, press

	Ctrl+C
