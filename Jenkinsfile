node('') {
stage 'buildInDevelopment'
openshiftBuild(namespace: 'development', buildConfig: 'mynginx', showBuildLogs: 'true')
stage 'deployInDevelopment'
openshiftDeploy(namespace: 'development', deploymentConfig: 'mynginx')
openshiftScale(namespace: 'development', deploymentConfig: 'mynginx',replicaCount: '1')
}
