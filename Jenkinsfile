node {
    
    stage('checkout') {
         git 'https://github.com/aishwaryavairagade/EMS-PUSHPENDRA.git'
    }
   
    stage('Hello') {
        echo 'Hello, Welcome to pipeline demo'
    }

     stage('build') {
        bat 'mvn clean install cobertura:cobertura'  
     }
     
     stage('Archive') {
        archiveArtifacts 'target/*.jar'

    }
}
