1. node.js
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
mkdir book1
mkdir book2
cd book1
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
build 后会生成_book
```sh
cd _book
python -m SimpleHTTPServer 4000
```
4. 预览
http://localhost:4000
