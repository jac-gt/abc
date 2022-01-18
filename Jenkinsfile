
pipeline {
  agent any
  stages {
    stage("build"){
      steps {
        echo 'Hello World'
        echo env.BRANCH_NAME
        script{
            def userStory = env.BRANCH_NAME.split('/')[1].trim().replace(' ',"_")
            println(userStory)
            env.USER_STORY=userStory         
        }
        echo env.USER_STORY
      }
    }
  }
}
