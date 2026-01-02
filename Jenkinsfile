@Library('jenkins-shared-library') _

properties([
    parameters([
        string(name: 'appVersion', defaultValue: ''),
        choice(name: 'Environment', defaultValue: 'dev')
    ])
])

def configmap = [
    appVersion = "${params.appVersion}"
    project = "roboshop"
    component = "catalogue"
    Environment = "${params.Environment}"
]

EKSdeploy.groovy