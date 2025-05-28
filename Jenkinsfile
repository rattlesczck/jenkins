pipeline {
    agent any
    
    parameters {
        string(name: 'NUMBER1', defaultValue: '5', description: 'First number to add')
        string(name: 'NUMBER2', defaultValue: '3', description: 'Second number to add')
    }
    
    stages {
        stage('Calculate Sum') {
            steps {
                script {
                    // Convert string parameters to integers and calculate sum
                    def num1 = params.NUMBER1.toInteger()
                    def num2 = params.NUMBER2.toInteger()
                    def sum = num1 + num2
                    
                    // Output the result
                    echo "The sum of ${num1} and ${num2} is: ${sum}"
                }
            }
        }
    }
} 