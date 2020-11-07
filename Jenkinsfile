pipeline{
agent any
  
stages{
stage("build"){
steps{
echo "building"
}
}
  stage("test"){
    when{
      expression{
        BRANCH_NAME == "DEV"
      }
    }
steps{
echo "Testing"
}
}
}
}
