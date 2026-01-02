@Library('jenkins-shared-library') _

properties([
    parameters([
        string(name: 'appVersion'),
        choice(name: 'environment', defaultValue: 'dev')
    ])
])

def configmap = [
    appVersion = "${params.appVersion}"
    project = "roboshop"
    component = "catalogue"
    environment = "${params.environment}"
]

eksdeploy.groovy