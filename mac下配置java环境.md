  1.  在JAVA官网下载最新版JDK，按步骤安装；
  2.  打开terminal，输入java -verision查看版本号   
（或者查看是否存在这个地址 **/Library/Java/JavaVirtualMachines/jdk-10.0.2.jdk/Contents/Home** )；

  3. 
```
sudo vim etc/profile
```
 在尾部输入如下语句

```
JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-10.0.2.jdk/Contents/Home
PATH=$JAVA_HOME/bin:$PATH:.
CLASSPATH=$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
export JAVA_HOME
export PATH
export CLASSPATH
```

  4. 输入 
```
source /etc/profile
```

  5. 检查是否成功 
```
echo $JAVA_HOME
```

显示如下，则表示成功

```
/Library/Java/JavaVirtualMachines/jdk-10.0.2.jdk/Contents/Home
```

  6. 编写第一个java文件， 保存为**HelloWorld.java**


```
public class HelloWorld {
   public static void main(String[] args) {
      // Prints "Hello, World" in the terminal window.
      System.out.println("Hello, World");
   }
```

}
  7. 编译 
```
javac HelloWorld.java
```

  8. 运行 
```
java HelloWorld
```


