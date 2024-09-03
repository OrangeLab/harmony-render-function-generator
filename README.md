# Hummer鸿蒙渲染函数生成插件
## 使用示例
```
const path = require('path')
const HarmonyRenderFunctionPlugin= require('@hummer/harmony-render-function-generator')


module.exports = {
  type: 'hummer',
  webpack: {
    // entries: "src/*/index.ts",
    entries: "src/*.js",
    output: {
      path: path.resolve(__dirname, './dist'),
      filename: "[name].js"
    },
    plugins: [
      new HarmonyRenderFunctionPlugin({
        wrapFunction: 'renderFunc'
      }),
    ]
  }
}
```

注意：需要发包
