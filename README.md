# appkit
AppKit is a collection of 28 developer utilities — encoders, hashes, formatters, timestamps, QR, Markdown/CSV editors and more. Everything runs client-side: your input never leaves the browser. Works offline.

# AppKit · 在线编码转换工具站

> 28 个开发者日常工具，**全部在浏览器本地计算，输入内容不上传到任何服务器**。
> 在线地址：https://www.appkit.top

## 为什么又做一个工具站

在线工具站很多，但大多数有两个问题：一是把你的内容 POST 到服务器上再算，
二是中文场景处理不了（GBK 乱码、中文转 UTF-8 结果不对）。
AppKit 想解决的就是这两点 —— **零上传**和**中文编码正确**。

## 功能

- **字符编码**：Ascii / Native 互转、Unicode 转义、UTF-8 编码
- **传输编码**：Base64（含图片 / 文件）、Base64URL、HTML 编码 / 解码、URL 编码 / 解码、二维码生成 / 解码
- **进制与字节**：Base-N 通用进制、Hex 编码 / 解码
- **时间**：Unix 时间戳
- **密码学**：对称加密、哈希算法、HMAC、密钥派生
- **代码保护与凭证**：JS 代码混淆、JS 混淆加密压缩、随机密码生成器
- **格式化**：CSS 格式化、文本内容对比、JS / HTML 格式化、JSON 格式化与压缩
- **网络工具**：域名注册状态查询、WHOIS 查询、ICP 备案查询、HTTP 请求模拟
- **在线编辑器**：Markdown 在线编辑器、CSV 在线编辑器

## 几个值得一提的

- **中文编码是真做了的**：GBK / GB2312 / Big5 / Shift_JIS 都有本地码表，
  「Native 编码」能正确在 GBK 与 UTF-8 之间互转，不是拿 `TextDecoder` 糊一下。
- **HTTP 请求模拟**：在浏览器里发请求，同时一键生成 cURL / JavaScript / Python / PHP
  四种语言的可用代码 —— 发送和代码生成共用同一份请求定义，不会出现「工具里发得通、
  粘出去发不通」。
- **CSV 编辑器**能识别乱码文件的真实编码，并给出两种解读让你自己选，不替你猜。
- 全部工具可离线使用，断网也能算。

## 技术栈

Vite 5 + Vue 3 + TypeScript(strict) + Tailwind。零后端，纯静态部署。

## 链接

https://www.appkit.top
