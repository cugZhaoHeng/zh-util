2024/04/12 发布了第一个版本，并成功上传到github上
> 【有道云笔记】发布自己的Maven仓库 https://note.youdao.com/s/cqPy3n48
（1）添加依赖
```xml
<dependency>
    <groupId>cn.perms</groupId>
    <artifactId>zh-util</artifactId>
    <version>1.0-SNAPSHOT</version>
</dependency>
```
（2）添加仓库
```xml
<repositories>
    <repository>
        <id>github</id>
        <url>https://maven.pkg.github.com/cugZhaoHeng/zh-util</url>
        <snapshots>
            <enabled>true</enabled>
            <updatePolicy>always</updatePolicy>
        </snapshots>
    </repository>
</repositories>
```
（3）在setting.xml中添加登录信息，因github不允许上传秘钥，所以只能使用图片的格式，自行使用ORC软件提取
![](./images/QQ截图20240412115245.png)