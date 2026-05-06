node{
    gti branch: 'main', url: 'https://github.com/Assem-Alasri/simple-java-app.git'
    stage('Bluid'){
        try{
            sh 'echo "Build stage"'
        }
        catch(Exception e){
            sh 'echo "Build stage failed"'
            throw e
        }
    }
    
    stage('Test'){
        if (env.BRANCH_NAME == "feat"){
            sh 'echo "test stage"'
        }
        else{
            sh 'echo "skip test stage"'
        }
    }
    
}