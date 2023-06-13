# Jenkinslib 使用说明

1. 创建/下载共享库
2. Jenkins 中配置 Library
   1. 共享库名称
   2. 共享库版本（master）
   3. 共享库地址
   4. 共享库凭据
3. Jenkinsfile 中加载共享库
   1. `@Library("name@version") _`
   2. `import org.devops.tools`
   3. `tools.printMsg("qingyun")`