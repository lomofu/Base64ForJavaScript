# Base64 For JavaScript
*Base64 For JavaScript which supports the Chinese*



### Quick Start

##### 1.在你的项目中引入Base64.js



##### 2.核心函数使用

```javascript
let data = '数据源data';

//编码 加密
let temp = encode64(strUnicode2Ansi(data));
// 解码 解密
let result = strAnsi2Unicode(decode64(result));
```

##### 3.服务端(java) 加密

```java
import java.io.IOException;
import org.apache.commons.codec.binary.Base64;
public class ZipStrUtil {    
    private static final String ENCODING_CHARSET = "GBK";
    
    //加密
    public static String deCompressBase64Zip(String compressedContent, String charset) throws IOException {
        byte[] decodeBase64 = Base64.decodeBase64(compressedContent);
        return new String(decodeBase64, charset);
    }
  }
}    
```

##### 5.参考demo