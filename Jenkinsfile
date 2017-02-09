try{
  node( test_cont_click){
    stage checkout 
    checkout scm
    
    stage buils & deploy 
    init_maven(
      sh mvn clean deploy 
    )
        
  
   
   
 }
}
catch(){
   
   
}
 
def init_maven(def body){
    def maven_version = tool name: '3.3.3'
    def java_version = tool name: '1.8'
    withEnv([ "JAVA_HOME=${maven_version}" "PATH+MAVEN=${maven_version}/bin"])
}
