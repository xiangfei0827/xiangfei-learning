# idea 注释配置

## 一、类头注释

打开file -> setting -> Editor -> Filr and Code Templates -> Includes -> File Header 

![类头注释.png](./../resource/微信截图_20191117212907.png "类头注释")

```
/**
 * description: 
 *
 * @author xiangfei
 * @date ${DATE} ${TIME}
 */
```

## 一、方法注释

打开 file -> setting -> Editor -> LiveTemplates

![方法注释步骤1.png](./../resource/微信截图_20191117213640.png "方法注释步骤1")

![方法注释步骤2.png](./../resource/微信截图_20191117213839.png "方法注释步骤2")

![方法注释步骤3.png](./../resource/微信截图_20191117213955.png "方法注释步骤3")

```
**
 * description: 
 * 
$param$ 
 * @return $return$
 */
```

![方法注释步骤4.png](./../resource/微信截图_20191117214140.png "方法注释步骤4")

```
groovyScript(         "def result='';          def params=\"${_1}\".replaceAll('[\\\\[|\\\\]|\\\\s]', '').split(',').toList();          for(i = 0; i < params.size(); i++) {             result +=' * @param ' + params[i] + ((i < params.size() - 1) ? '\\n' : '')};              return result ", methodParameters())
```

![方法注释步骤5.png](./../resource/微信截图_20191117214348.png "方法注释步骤5")