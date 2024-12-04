# Jenkins
<h3>GIT configuration to jenkins:</h3>
<h4>Ans: Go to global tool config > in the git section >Path to Git executable:put git path(by running whereis git  or simply put git)</h4>

<h3>Setup maven on jenkins:</h3>
<ul><h4>Install maven on jenkins: Download in /opt and extract it.</h4></ul>
<ul><h4>Setup env variables: JAVA_HOME, M2 and M2_HOME</h4></ul>
<p>open .bash_profile:</p>
<p>M2_HOME=/opt/maven</p>
<p>M2=/opt/maven/bin</p>
<p>JAVA_HOME=/usr/lib/jvm/java-11-openjdk-XXXX (it is jvm path it can be found byrunning command: find / -name java-11*)</p>
<p>PATH:$PATH:$HOME/bin:$JAVA_HOME:M2_HOME:M2</p>
<p>save the file and run : source .bash_profile and again run echo $PATH to see the path.</p>
<p>check : mvn -v</p>
<ul><h4>install maven plugin</h4></ul>
<p>Go to plugin section and install maven plugin</p>
<ul><h4>Configure maven and java</h4></ul>
<p>Go to global tool config > JDK > add JDK > JDK Name: java-11, JAVA_HOME: /usr/lib/jvm/java-11-openjdk-XXXX and uncheck install automatically.</p>

<p>Go to global tool config > Maven > add MVN >Maven Name: maven3.8.x, MAVEN_HOME: /opt/maven</p>
