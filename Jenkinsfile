pipeline {
agent any
stages {
stage ('Check') {
steps {
 println "appname:"+appname
 sh "sed -i 's/${appname}/Tomcat/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/tasks/main.yml"
 sh "ansible-playbook main.yml -u root"
 }
 }
 }
 }
