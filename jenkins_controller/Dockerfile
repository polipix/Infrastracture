FROM jenkins/jenkins:2.319.3-lts-jdk11
COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
ENV CASC_JENKINS_CONFIG /usr/share/jenkins/ref/casc.yaml
RUN jenkins-plugin-cli -f /usr/share/jenkins/ref/plugins.txt