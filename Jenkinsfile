// 加载共享库
@Library("mylib@master") _
import org.devops.tools

def tools = new tools()

pipeline {
    agent { label "worker1" }
    
    options {
        skipDefaultCheckout true
    }
    
    stages {
        stage("build") {
            steps {
                script {
                    // 使用类中的方法
                    tools.printMsg("hello world")
                    
                    // 执行demoPipeline
                    demoPipeline()
                }
            }
        }
    }
}
