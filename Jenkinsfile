pipeline{
agent any
tools{
gradle 'Gradle'
jdk 'JDK'
}
stages{
stage('Checkout'){
steps{
git branch:'master',url:'https://github.com/sinchanam12/sinchgradle.git'
}
}
stage('Build'){
steps{
sh'gradle build'}
}
stage('Test'){
steps{
sh'gradle test'}
}
stage('Run Application'){
steps{
sh'gradle run'}
}
}
post{
success{
echo'build successful'
}
failure{
echo'build failed'
}
}
}
