
 def workspace;
node{
    stage('checkout')
    {
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '03bdf51b-d21c-44c4-ac91-4de85e2d365a', url: 'https://github.com/belennae/apiConnect.git']]])
       workspace=pwd[]
    }
    stage('Static Code Analysis'){
        echo "Static Code Analysis"
    }
    stage('Build'){
        echo "Build the code"
    }
    stage('Unit Testing'){
        echo "Unit Testing"
    }
    stage ('Delivery'){
        echo "Delivery the code"
    }
}
