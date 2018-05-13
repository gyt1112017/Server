# Server


<h1>Technical Guide for Web & GIS app development project </h1>
<p style="font-family:calibri;font-size:150%;"> 
          This project consists of 3 components; the Server, question-app and the Quiz-app. The  three repositories together allow to create a location-based quiz. The project is also supported by data from postgreSQL/PGAdmin4 - which stores the data created/used in this project.</p>
          <p style="font-family:calibri;font-size:150%;"> 
            The following instruction is to make shure the app work well. </p>
          
<h2> NodeJS Server: httpServer </h2>
          <p style="font-family:calibri;font-size:150%;"> 
                                                        The Server repository consists of server-side code to 
                                                        process, upload/download and store data in both the web and mobile
                                                        applications. A HTTP server is used for both the Quiz-app and question-app as a result of a lack certification in HTTPS servers. GET and POST commands are used to download and upload data in both the Quiz-app and question-app</p>

<h3> Installation Guide </h3>
          <p style="font-family:calibri;font-size:150%;">
          <ul>
          <li>Install the Server repository by going on terminal and typing: git clone https://github.com/gyt1112017/Server.git </li>
          <li>Go to the Server directory using the terminal: "~/code/Server"</li>
          <li>To run the server, type: "node httpServer.js &". The addition of the '&' allows the server to run in the background.</li>
          <li>In order to stop running the servers, type: "fg 1" which will display the current running servers and then type :"Ctrl+C". 
          <li> Having run the httpServer.js in the background, navigate to a phonegap app directory e.g. question-app, inside the uczlyg5 folder and type: phonegap serve
          </li>
            <li>Once the phonegap server is running successfully go to: http://developer.cege.ucl.ac.uk:31273/</li>
          <li>To stop the phonegap server, press Ctrl+C.</li>
          </ul></p>

<h3> Technical Information </h3>
<p style="font-family:calibri;font-size:150%;">
The following port numbers were used in the project and are assigned to each server:
<ul>
          <li>HTTP: 30273</li>
          <li>HTTPS: 31073</li>
          <li>Phonegap: 31273</li>
                                                  
<h2> Web Application: question-app </h2>
<p style="font-family:calibri;font-size:150%;"> 
  The question-app part is for use in a web browser, accessible to the creators/administrators of the project. </p>

<h3> Installation Guide </h3>
<p style="font-family:calibri; font-size:150%;">
<ul>
<li>Install the 'question-app' repository by going on terminal and typing: git clone https://github.com/gyt1112017/question-app.git </li>
<li> Before you run the app, you need to run the httpServer.js in the background, which is in the Server file.</li>
<li> Go to the question-app directory and run the phonegap server: "~/code/question-app/uczlyg5" and enter "phonegap serve"</li>
<li> In one of the specified ports highlighted in the technical information section, use the following URL to load the app: http://developer.cege.ucl.ac.uk:31273/ </li>
<li>To understand how to use this app, go to: http://developer.cege.ucl.ac.uk:31273/user-guide.html </li></ul></p>

<h3> Technical Information </h3>
<p style="font-family:calibri; font-size:150%;"> 
This app was tested using the following browsers:
          <ul>
          <li>Google Chrome v66.0.3359.139 (Official Build) (64-bit)</li>
          <li>Microsoft Edge v41.16299.371.0</li>
          </ul></p>

<h2>Mobile Application: Quiz-app </h2>
<p style="font-family:calibri;font-size:150%;">The Quiz-app is created specifically for use on an android mobile devices,  and the users are required to connect to the UCL VPN network.</p>

<h3> Installation Guide </h3>
<p style="font-family:calibri; font-size:150%;">
<ul>
<li> Install the 'Quiz-app' repository by going on terminal and typing: git clone https://github.com/gyt1112017/Quiz-app.git </li>
<li> To run the app - the httpServer.js from the section above needs to be installed and running in the background. </li>
<li> Go to the Quiz-app directory and run the phonegap server: "~/code/Quiz-app/uczlyg5" and enter "phonegap serve"</li>
<li> In one of the specified ports highlighted in the technical information section, use the following URL to load the app: http://developer.cege.ucl.ac.uk:31273/ </li>
<li> To understand how to use this app, go to: http://developer.cege.ucl.ac.uk:31273/user-guide.html </li></ul></p>

<h3> Technical Information </h3>
<p style="font-family:calibri; font-size:150%;"> 
This app was tested using the following browsers:
          <ul>
          <li>Google Chrome v66.0.3359.139 (Official Build) (64-bit)</li>
          <li>Microsoft Edge v41.16299.371.0</li>
          </ul>
And the following mobile operating system:
          Android Marshmallow 6.0.1</p>

<li>Code adapted from: https://github.com/claireellul/cegeg077-week5server/blob/master/httpServer.js</li>
<li>Code adapted from: https://github.com/claireellul/cegeg077-week5app/blob/master/ucfscde/www/js/appActivity.js</li>
<li>Code adapted from: https://github.com/claireellul/cegeg077-week6formcode</li>
