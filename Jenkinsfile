#!groovy
@Library('roboshop-shared-library') _

//resposibility to pass what type of application and component is this to pipeline decission

def configMap = [
    application: "nodejsVM",
    component: "user"
]

if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pipelineDecission.decidePipeline(configMap)

}
else{
    echo "this is PRODUCTION, deal with CR process"

}