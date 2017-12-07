pipeline {
    agent any
   
    parameters{

booleanParam(defaultValue: true,description: '',name:'boolean_param')
string(defaultValue:"this is to test string parameter",description:'No description',name:'string_param')
choice(choices: 'choice1\nchoice2\nchoice3',description: 'this is demo of choice pipeline parameter',name: 'choice_param') 

}
  


    stages {
        stage('boolean') {
            steps {
                echo 'calling boolean parameter  ${params.boolean_param}'
            }
        }
        stage('string') {
            steps {
                echo 'calling string parameter ${params.string_param}'
            }
        }
        stage('Deploy') {
            steps {
                echo 'calling choice parameter ${params.choice_param}'
            }
        }
    }
}
