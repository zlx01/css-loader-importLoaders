# css-loader

## 实验结果

1.对于scss文件，因为sass-loader会处理好@import，所以importLoaders配置无关紧要

2.importLoaders不配置或者设置为0时，只有第一层@import的css会添加厂商前缀

3.importLoaders设置为1时，嵌套引入的css也会添加产商前缀

```bash
npx postcss src/*.css --use autoprefixer -d dist/
```

## Reference

* https://kelly-kh-woo.medium.com/webpack-css-loader-importloaders-e8e23decd900
* https://stackoverflow.com/questions/52544620/what-is-exactly-the-importloaders-option-of-css-loader-in-webpack-4


