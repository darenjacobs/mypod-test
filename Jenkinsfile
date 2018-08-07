podTemplate(label: 'jenkins-node',
) {
    node ('jenkins-node') {
        stage ('Switch to Utility Container') {
           container('jenkins-node') {
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
