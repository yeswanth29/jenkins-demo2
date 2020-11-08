pipeline{
agent any
  parameters{
 
    choice(name:"Version",choices:['1.02','10.2'],description:"")
    booleanParam(name:"environ",defaultValue:true,description:"")
stages{
stage("build"){
steps{
echo "building"
}
}
  stage("test"){
    when{
      expression{
        params.environ
      }
    }
steps{
echo "Testing"
  echo "Building with ${params.Version}"
}
}
}
}
