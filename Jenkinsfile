podTemplate(label: 'jenkins-pod',
) {
    node ('jenkins-pod') {
        stage ('Switch to Utility Container') {
           container('jenkins-pod') {
             sh ("echo 'Hello World!'")
             sh ("ansible --version")
             sh ("ant -version")
             sh ("jq --version")
             sh ("mvn --version")
             sh ("packer --version")
             sh ("whoami")
             sh ("id -u jenkins")
             sh ("env")
             sh ("sleep 30")
           }
        }
    }
}
