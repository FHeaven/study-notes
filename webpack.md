### npm package.json 
#### 关于script
``` javascript
{
  "name": "01.start",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start": "webpack"
    // "heaven":"webpack" // 不一定用start, 使用其他的名字，则npm run heaven
  },
  "author": "Heaven Fan",
  "license": "ISC",
  "devDependencies": {
    "webpack": "^3.10.0"
  }
}
```




Web应用的复杂性 -->  Solution的改进 --> 模块化编程的产生；编程语言的产生；CSS预编译器的产生  -->  为了让浏览器识别，需要额外处理 --> webpack的产生；为模块打包而生；找到浏览器不可识别的扩展语言，找到模块，转化为浏览器可识别的格式。


把你的项目当做一个整体，通过一个给定的主文件（如：index.js），Webpack将从这个文件开始找到你的项目的所有依赖文件，使用loaders处理它们，最后打包为一个（或多个）浏览器可识别的JavaScript文件

cnpm install -g webpack
cnpm install --save-dev webpack
cnpm install --save-dev webpack-dev-server

cnpm init

允许开发者模式，有原文档进行DEBUG
devtool: 'eval-source-map'

// 修改代码立刻反应到UI
devServer: {
 contentBase: '相对url',
 port: '8080',
 inline: true,
 historyApiFallBack: true

}

contentBase	默认webpack-dev-server会为根文件夹提供本地服务器，如果想为另外一个目录下的文件提供本地服务器，应该在这里设置其所在目录（本例设置到“public"目录）
port	设置默认监听端口，如果省略，默认为”8080“
inline	设置为true，当源文件改变时会自动刷新页面
historyApiFallback	在开发单页应用时非常有用，它依赖于HTML5 history API，如果设置为true，所有的跳转将指向index.html

作者：zhangwang
链接：http://www.jianshu.com/p/42e11515c10f
來源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。



package.json
"scripts": {
 "start":"webpage",
 "server":"webpack-dev-server --open"
}

Loaders是webpack的核心组成部分，使用不同的loaders，实现不同格式文档的处理。(SASS, LESS, React的JSX)
test：一个用以匹配loaders所处理文件的拓展名的正则表达式（必须）
loader：loader的名称（必须）
include/exclude:手动添加必须处理的文件（文件夹）或屏蔽不需要处理的文件（文件夹）（可选）；
query：为loaders提供额外的设置选项（可选）


Babel是Loaders之所以能解析不同的file的条件：
解析Es6的babel-env-preset包和解析JSX的babel-preset-react包
Babel的安装：
npm install --save-dev babel-core babel-loader babel-preset-env babel-preset-react
