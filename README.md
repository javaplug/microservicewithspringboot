# microservicewithspringboot
Microservices with Springboot

Spring Boot [Framework for developing web application]
======================================================
opinionated     - comes with a lot of non-functional features, quick development
configuration   - can be overriden any of the opinionated features
Embedded-server - gives stand-alone jar/war with embedded Tomcat server

Getting Started
===============
Tools required
 - Java 8 [Programming language]
   - http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
   - Click 'Accept License Agreement' and Download a JDK [Java SE Development Kit 8u] which suites your OS
   - Install
 - Spring-tool-suite(STS) [Editor]
   - https://spring.io/tools/sts/all
   - Download and Install
 - Apache Maven [Build tool]
   - https://maven.apache.org/download.cgi
   - Download a binary file by making sure that file name has [-bin], sample file name -> apache-maven-3.5.x-bin.zip
   - unzip that anywhere in your PC
 - [Optional] Git [Source Control Management tool]
   - https://git-scm.com/downloads
   - Download and Install
 - [Optional] Postman [API Development Environment]
   - https://www.getpostman.com/apps
   - Download and Install
   - open postman, if you want to take backup of your data, you can sign-in otherwise click 'Take me straight to the app..'

Configuration
=============
 - Set below Environmet Variables
   - M2_HOME = ~/apache-maven-3.6.0
   - JAVA_HOME = C:\Program Files\Java\jdk-10.0.1
   - PATH = all-existing-setting-keep-as-is;%JAVA_HOME%\bin;%M2_HOME%\bin
 - Open STS
 - it asks a path for creating a workspace, choose a folder your PC
 - it opens the workspace
 - setting maven
   - from menu option click: Window -> Preferences -> [in left-panel]Maven : Installations -> [in right-panel] click 'Add' : click 'Directory' and choose the folder where you unziped 'Apache Maven' '~\apache-maven-3.5.3' and click : 'Finish'
   - from menu option click: Window -> Preferences -> [in left-panel]Maven : 'User Settings' -> [in right-panel] click 'Browse' : and choose '~\apache-maven-3.5.3\conf\settings.xml' and click : 'Apply and close'

Importing Maven Project and starting
====================================
  - Right click inside 'Package Explorer' -> 'Import..' -> 'Maven' -> 'Existing Maven Projects' -> choose 'ws_teammgmt_team' -> click : 'Finish'
  - Boot dashboard
    - from menu option click: 'Window' -> 'Show View' -> 'Other..' -> type 'boot' -> click : 'Open'
  - In boot dashboard expand 'local' -> choose 'ws_masterdata_team' -> right click -> (Re)start/(Re)debug
  - once app started you can see the console log
      Tomcat started on port(s): 8080 (http) with context path ''
      Started MasterdataTeamApplication in 20.906 seconds (JVM running for 28.587)
  - make a note of the port 8080, it might change use accordingly
  - open postman and give input as per 'tutorials/postmanrequest.PNG' in the same page -> scroll-up and click 'Send'
  - you can see the success message in the same window as highlighted in red 'tutorials/postmanrequest.PNG'
  - in browser open 'http://localhost:8080/h2-console' and give input as per 'tutorials/h2console.PNG' and click 'connect'
  - this is a console of embedded db configured in the ws_masterdata_team
  - sample usage refer 'tutorials/output.PNG'

<End of Environment setup>
