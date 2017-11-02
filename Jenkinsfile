node ("master") {
stage ("SCM"){
    git 'https://github.com/nthota0/MavenRepo_New.git'
}
stage ("BUILD"){
   sh 'mvn clean compile package'
}
stage ("Deploy"){
   sh 'mvn deploy'
}
stage ("Test"){
   echo 'build'
}}
