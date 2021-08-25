# file-manage-js
文件管理相关方法


## Install

```
npm install file-manage-js -D
```

### Use

```javascript
const fileManager = require('file-manage-js')

console.log(fileManager.existsSync('./existsSync.js')) // { code: 200, data: { type: 'file' }, message: '' }

;(async function() {
  const res = await fileManager.exists('./existsSync.js')
  console.log(res) // { code: 200, data: { type: 'file' }, message: '' }
})()
```


### Api
``` javascript
  fileManager.existsSync // 判断目录是否存在（同步）
  fileManager.exists // 判断目录是否存在
  fileManager.fileHasSync // 判断文件是否存在（同步）
  fileManager.fileHas // 判断文件是否存在
  fileManager.dirHasSync // 判断文件夹是否存在（同步）
  fileManager.dirHas // 判断文件夹是否存在
  fileManager.readDirSync // 读取文件目录（同步）
  fileManager.readDir // 读取文件目录
  fileManager.deletePathSync // 删除(文件|文件夹)（同步）
  fileManager.deletePath // 删除(文件|文件夹)
  fileManager.mkDirSync // 创建文件夹（同步）
  fileManager.mkDir // 创建文件夹
  fileManager.writeFileSync // 创建/修改文件(覆盖)（同步）
  fileManager.writeFile // 创建/修改文件(覆盖)
  fileManager.appendFileSync // 创建/追加文件（同步）
  fileManager.appendFile // 创建/追加文件
  fileManager.readFileSync // 读取文件（utf-8）（同步）
  fileManager.readFile // 读取文件（utf-8）
  fileManager.copySync // 拷贝(文件|文件夹)（同步）
  fileManager.copy // 拷贝(文件|文件夹)
```


## License

The MIT License. Full License is [here](https://github.com/mj132/file-manage-js/blob/main/LICENSE)
