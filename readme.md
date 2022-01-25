## Prerequisite

  * JDK 1.8

## Download versi portable (Binary Zip)

  * Apache Netbeans 12 (Recommended) : [https://netbeans.apache.org/download/nb120/nb120.html](https://netbeans.apache.org/download/nb120/nb120.html)
 
  * or Apache Netbeans 11 (Old but still work) : [https://netbeans.apache.org/download/nb110/nb110.html](https://netbeans.apache.org/download/nb110/nb110.html)

  * Apache Tomcat : [https://tomcat.apache.org/download-90.cgi](https://tomcat.apache.org/download-90.cgi)

## Limit Memory Usage Netbean

  * Update file [Dir Netbean Portable]/etc/netbeans.conf

![Image](https://raw.githubusercontent.com/si294r/netbean/master/netbeans.conf.png)

## Tools > Options > Java > Maven

![Image](https://raw.githubusercontent.com/si294r/netbean/master/tools-options-java-maven.png)

## Tools > Options > Java > Java Debugger

![Image](https://raw.githubusercontent.com/si294r/netbean/master/tools-options-java-debugger.png)

## Tools > Options > Editor > Formatting

![Image](https://raw.githubusercontent.com/si294r/netbean/master/tools-options-editor-formatting.png)

## Tools > Options > Editor > Code Completion

![Image](https://raw.githubusercontent.com/si294r/netbean/master/tools-options-editor-codecompletion.png)

## Tools > Plugins > Available Plugins > NB SpringBoot

![Image](https://raw.githubusercontent.com/si294r/netbean/master/tools-plugins-springboot.png)

## Services > Servers > Apache Tomcat

![Image](https://raw.githubusercontent.com/si294r/netbean/master/services-servers-tomcat.png)

## Project > Properties > Build > Compile

![Image](https://raw.githubusercontent.com/si294r/netbean/master/project-properties-build-compile.png)

## Project > Properties > Run

![Image](https://raw.githubusercontent.com/si294r/netbean/master/project-properties-run.png)

## Speed up debug time

Find file catalina.bat in your tomcat folder (ex: D:\apache-tomcat-8.5.53\bin\catalina.bat), then add command to delete project alamisharia deployment 
right after line setlocal

```
rem   TITLE           (Optional) Specify the title of Tomcat window. The default
rem                   TITLE is Tomcat if it's not specified.
rem                   Example (all one line)
rem                   set TITLE=Tomcat.Cluster#1.Server#1 [%DATE% %TIME%]
rem ---------------------------------------------------------------------------

setlocal

del "%cd%\..\conf\Catalina\localhost\alamisharia.xml"

```
this will skip undeployment process and speed up debug time



## PROBLEM cannot run cmd !!!

[https://stackoverflow.com/questions/58445540/netbeans-9-10-11-cannot-run-program-cmd](https://stackoverflow.com/questions/58445540/netbeans-9-10-11-cannot-run-program-cmd)

![Image](https://raw.githubusercontent.com/si294r/netbean/master/problem_cannot_run_cmd.png)
