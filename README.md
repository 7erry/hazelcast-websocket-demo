
To run this demo you'll need a copy of Tomcat or another Web Container with support for JSR-356.

Build the project with `mvn clean install -DskipTests`<br/>

Start the test:<br/>
mvn tests<br/>

Install Tomcat webserver:<br/>
OSX>brew install tomcat<br/>

Add a user to the manager-gui if you wish to deploy the war file dynamically:<br/>
OSX>vi /Users/yournamehere/homebrew/Cellar/tomcat/9.0.16/libexec/conf/tomcat-users.xml<br/>

Start tomcat in the foreground (testing purposes)<br/>
OSX>catalina run<br/>

Deploy /hazelcast-web<br/>
http://localhost:8080/manager/html<br/>

Load up the stockticker.jsp<br/>
open http://localhost:8080/hazelcast-web/stockticker.jsp<br/>

Load up the Swing consumer:<br/>
hazelcast-client/controller.Controller.main<br/>

<br/>
![alt text](https://raw.githubusercontent.com/7erry/hazelcast-websocket-demo/images/SwingInterface.png)<br/>
![alt text](https://raw.githubusercontent.com/7erry/hazelcast-websocket-demo/images/WebInterface.png)<br/>
![alt text](https://raw.githubusercontent.com/7erry/hazelcast-websocket-demo/images/TestDataOutput.png)<br/>
<br/>
