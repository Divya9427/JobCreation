pipeline {
agent any
stages {
stage ('Check') {
steps {
 println "appname:"+appname
 sh "sed -i 's/${appname}/java_pipeline/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/tasks/main.yml"
 sh "ansible-playbook main.yml"
 }
 }
 }
 }
