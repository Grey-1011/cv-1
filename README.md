# 部署方式
每次改完代码，必须运行这一行，才能正确的请求 JS 和 CSS

```
parcel build src/index.html --no-minify --public-url .
```
# 如果部署时出现 No such file or directory
请 Delete .parcel-cache and dist (只适用于 version 1.x of parcel 版本)，代码如下：
```
rm -rf .parcel-cache dist
npm run cleanup && parcel ./index.html
```

