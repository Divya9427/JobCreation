pipeline {
agent any
stages {
stage ('Check') {
steps {
 println "appname:"+appname
 sh "sed -i 's/${appname}/Tomcat/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/tasks/main.yml"
 sh "sed -i 's/${giturl}/gitlink/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/files/template.xml"
 sh "sed -i 's/${branchname}/mybranch/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/files/template.xml"
 sh "ansible-playbook main.yml -u root"
 }
 }
 }
 }
