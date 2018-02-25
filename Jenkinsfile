node {
    stage('checkout'){
       checkout([$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '5fe8635c-4906-43f1-9b91-01dcbf36cd88', url: 'https://github.com/rita19872/maven-single-module.git']]])
    }
    stage('build'){
       //sh " mvn clean install "
      bat( /mvn clean install/) 
    }
}
