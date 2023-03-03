# FormDataPolyfill


### 怎么用

```shell
npm install @macrocc/formdata-polyfill
```

```javascript
import FormData from '@macrocc/formdata-polyfill'
const formData = new FormData((path) => Taro.getFileSystemManager().readFileSync(path), fields)
formData.appendFile('files',path)
const [data, contentType] = formData.generate()
fetch(url , data,{ contentType }, "POST");
```


## 感谢来自 https://github.com/zlyboy/wx-formdata 的参考