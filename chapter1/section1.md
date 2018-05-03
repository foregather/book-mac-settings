1. node.js和npm
2. gitbook
  - 安装
```sh
npm install -g gitbook-cli
```
  - 查看版本
```sh
gitbook -V
```
3. 创建目录结构
```sh
mkdir book
cd book
touch README.md
touch SUMMARY.md
vi SUMMARY.md
```
4. 目录结构
```sh
tree
```
```sh
.
├── README.md
├── SUMMARY.md
├── chapter1
│   ├── README.md
│   ├── section1.md
│   └── section2.md
├── chapter2
│   ├── README.md
│   ├── section1.md
│   └── section2.md
└── end
    └── README.md
```
5. SUMMARY.md 例子
  ```sh
  * [简介](README.md)

  * [第一章](chapter1/README.md)

   - [第一节](chapter1/section1.md)

   - [第二节](chapter1/section2.md)

  * [第二章](chapter2/README.md)

   - [第一节](chapter2/section1.md)

   - [第二节](chapter2/section2.md)

  * [结束](end/README.md)
  ```

6. 启动
  - 方式一
```sh
gitbook build
gitbook serve
```
  - 方式二
gitbook build 后会生成[_book](#jump)
```sh
cd _book
python -m SimpleHTTPServer 4000
```
7. 预览
http://localhost:4000

8. 创建github账号，将book同步到github
9. 创建gitbook账号，新建Organizations，新建Space，创建完把该space和github链接起来，以后写完提交到github后自动同步到gitbook，设置如下图：

![](https://ws3.sinaimg.cn/large/006tNc79ly1fqy78mvae8j318s0mm415.jpg)

![](https://ws1.sinaimg.cn/large/006tNc79ly1fqy79hi9emj31gs0dojsw.jpg)
