pipeline {
    agent any
    stages {
        stage('Branch Info') {
            steps {
                echo "🚨 Running on branch: ${env.BRANCH_NAME}"
            }
        }
        stage('Branch-Based Step') {
            steps {
                script {
                    if (env.BRANCH_NAME == "main") {
                        echo "🚀 Production Deployment"
                    } else if (env.BRANCH_NAME.startsWith("feature")) {
                        echo "🧪 Feature Branch Build"
                    } else {
                        echo "🔧 Misc branch build"
                    	echo "📝 Code updated and pushed!" 
}
                }
            }
        }
    }
}

