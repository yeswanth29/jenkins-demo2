pipeline{
agent any
  parameters{
 
    choice(name:"Version",choices:['1.02','10.2'],description:"")
stages{
stage("build"){
steps{
echo "building"
}
}
  stage("test"){
    
steps{
echo "Testing"
  echo "Building with ${params.Version}"
}
}
}
}
