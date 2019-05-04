node {
 stage('scm check')
 {
 git 'https://github.com/javahometech/my-app.git'
 }
 stage ('build package')
 {
 def  Home = tool name: 'MK_firsttest', type: 'maven'
  sh "${Home}/bin/mvn package"
 }

}
