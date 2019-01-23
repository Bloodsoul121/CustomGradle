# CustomGradle
自定义插件

编辑build.gradle文件，如下：

apply plugin: 'groovy'
apply plugin: 'maven'
 
dependencies {
    compile gradleApi()
    compile localGroovy()
}
repositories {
    mavenCentral()
}

添加依赖：

dependencies {
    classpath 'com.custom.gradle.plugin:time:1.0.0'
}

或

dependencies {
    classpath files('libs/time-1.0.0.jar')
}

参考学习网址：https://blog.csdn.net/a646796992/article/details/82259502
