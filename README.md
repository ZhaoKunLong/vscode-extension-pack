# install package

1. 安装在全局。 可以直接使用。
```sh
    npm install -g yo generator-code
```

2. 然后在当前路径生成

```sh
yo code
选择使用 extension pack
```

3. 如果 code no find.

[code-is-not-working-in-on-the-command-line-for-visual-studio-code-on-os-x-ma](https://stackoverflow.com/questions/29955500/code-is-not-working-in-on-the-command-line-for-visual-studio-code-on-os-x-ma)


4. 进入到 生成的pack 文件。查看 package.json 
5. 直接编辑 package.json 里面的 extension pack 来进行 extension的包含

6. 安装 vsce
```sh
npm i -g vsce 
```
7. 生成本地包
```sh
cd <pack>
vsce package  // 会打包生成
```

8. 装载到本地
```sh
code --install-extension <the file name of vsix>
```
9. 拿到 personal access token
```sh
vsce publish // 推送到 市场
```