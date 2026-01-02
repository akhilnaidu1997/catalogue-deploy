@Library('jenkins-shared-library') _

properties([
    parameters([
        string(name: 'appVersion', defaultValue: ''),
        choice(name: 'environment', defaultValue: 'dev')
    ])
])

def configmap = [
    appVersion = "${params.appVersion}"
    project = "roboshop"
    component = "catalogue"
    Environment = "${params.environment}"
]

EKSdeploy.groovy