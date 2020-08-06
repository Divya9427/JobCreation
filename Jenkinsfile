pipeline {
agent any
stages {
stage ('Create Pipeline') {
steps {
 sh "sed -i 's/Tomcat/${appname}/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/tasks/main.yml"
 sh "sed -i 's,http://gitlink123,${giturl},g' ${WORKSPACE}/roles/Jenkins_Job_Creation/files/template.xml"
 sh "sed -i 's/mybranch/${branchname}/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/files/template.xml"
 sh "ansible-playbook main.yml -u root"
 }
 }
 }
 }
