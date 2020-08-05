pipeline {
agent any
stages {
stage ('Check') {
steps {
 sh "sed -i 's/${appname}/java_pipeline/g' ${WORKSPACE}/roles/Jenkins_Job_Creation/tasks/main.xml ansible-playbook main.yml"
 }
 }
 }
 }
