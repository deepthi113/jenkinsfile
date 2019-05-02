node {
    stage ("scm")
    {
    git 'https://github.com/ghanigreen/maven_demo.git'
    }
    stage ("build")
    {
    sh 'mvn package'
    }    
    stage ("deploy")
    {
        sh sudo su
        sh 'cp -R "/var/lib/jenkins/workspace/jenkins/gameoflife-web/target/gameoflife.war" "/usr/share/tomcat/webapps"'
    }

    
    
}
