node {
    stage('Initialization') {
        sh 'echo dummy step'
        sh 'sleep 20'
    }

    stage('Testing'){
        parallel centos:{
            node('centos'){
                sh 'echo Hello from Centos'
                sh 'sleep 30'
            }
        },
        ubuntu:{
            sh 'echo Hello from ubuntu'
            sh 'sleep 30'
        }
         
    }
    stage('Notify People'){
        sh 'echo hello people'
    }
    stage('Notify People2'){
        sh 'echo hello people'
    }
    //
}