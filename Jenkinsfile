¨node {
    
    stage ('checkout'){
        
    git 'https://github.com/javahometech/my-app.git'
        
        }
    stage('mvn package'){
    
    def maven_home= tool name: 'MAVEN_HOME', type: 'maven'
    def mvn_cmd = "${maven_home}/bin/mvn"
    "${mvn_cmd} mvn clean package"
    }
