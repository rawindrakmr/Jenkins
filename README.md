# Jenkins
<h3>GIT configuration to jenkins:</h3>
<h4>Ans: Go to global tool config > in the git section >Path to Git executable:put git path(by running whereis git  or simply put git)</h4>

<h3>Setup maven on jenkins:</h3>
<ul>Install maven on jenkins: Download in /opt and extract it.</ul>
<ul>Setup env variables: JAVA_HOME, M2 and M2_HOME</ul>
open .bash_profile:
M2_HOME=/opt/maven
M2=/opt/maven/bin
JAVA_HOME=/usr/lib/jvm/java-11-openjdk-XXXX (it is jvm path it can be found byrunning command: find / -name java-11*)
PATH:$PATH:$HOME/bin:$JAVA_HOME:M2_HOME:M2
save the file and run : source .bash_profile and again run echo $PATH to see the path.
check : mvn -v
<ul>install maven plugin</ul>
Go to plugin section and install maven plugin
<ul>Configure maven and java</ul>
Go to global tool config > JDK > add JDK > JDK Name: java-11, JAVA_HOME: /usr/lib/jvm/java-11-openjdk-XXXX and uncheck install automatically.

Go to global tool config > Maven > add MVN >Maven Name: maven3.8.x, MAVEN_HOME: /opt/maven
