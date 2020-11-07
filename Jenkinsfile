pipeline{
agent any
  parameters{
    string(name:"Version", defaultValue:'', description:"thids is version")
    choice(name:"Version", choices:['1.0.1','1.245'],description:'')
  }
stages{
stage("build"){
steps{
echo "building"
}
}
  stage("test"){
    when{
      expression{
        params.Version =='1.0.1'
      }
    }
steps{
echo "Testing"
}
}
}
}
