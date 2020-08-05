pipeline {
agent any
stages {
stage ('Check') {
steps {
 println "appname:"+appname
 sh "sed -i 's/Tomcat/${appname}/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/tasks/main.yml"
 sh "sed -i 's/<url>gitlink123</url>/<url>${giturl}</url>/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/files/template.xml"
 sh "sed -i 's/mybranch/${branchname}/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/files/template.xml"
 sh "ansible-playbook main.yml -u root"
 }
 }
 }
 }
