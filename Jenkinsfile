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
        sh 'cp -R "C:\\Program Files (x86)\\Jenkins\\workspace\\jenkin demo\\gameoflife-web\\target\\gameoflife.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps"'
    }

    
    
}
