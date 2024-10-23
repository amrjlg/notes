# gradle

## 版本升级到7.x之后

- dependencies变化

```groovy
dependecies {
    compile('xxx')
}
```

```groovy
dependecies {
    implementation('xxx')
}
```

- 证书信任配置
在gradle.properties加入下列配置
```properties
systemProp.javax.net.ssl.trustStore=path/to/trust/store
systemProp.javax.net.ssl.trustStorePassword=yourpassword
```
trust store 文件可以使用jdk自带的`keytool`工具生成

```shell
keytool -import \
  -alias alias \
  -keystore cacerts \
  -storepass changeit \
  -noprompt \
  -file ca.pem
```
注意上面 -alias 参数，这个是给证书取个别名；-file 参数，指定的是 CA 证书的路径。

- 获取ca证书的方法

在chrome/edge中打开指定域名的一个网页，在地址栏https前面的安全锁出点击查看证书，导出为pem证书即可