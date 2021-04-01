# 使用 husky eslint commitlint 等工具统一项目规范

<!-- > 之前做的项目,大多都是通过脚手架直接生成的自带了 eslint commitlint 等开发的一些规范 ,  -->

## 官网文档

- [commit lint](https://commitlint.js.org/#/)
- [husky](https://typicode.github.io/husky/#/?id=automatic-recommended)
- [prettier](https://prettier.io/)
- [eslint](http://eslint.cn/docs/user-guide/command-line-interface)
- [lint-staged](https://github.com/okonet/lint-staged#readme)

## lint-staged

在代码提交之前，进行代码规则检查能够确保进入git库的代码都是符合代码规则的。但是整个项目上运行lint速度会很慢，lint-staged能够让lint只检测暂存区的文件，所以速度很快。

``` json  
{
  "lint-staged": {
    "src/*.{js,jsx,ts}": "eslint"
  }
}
```

## 参考资料

- [使用ESLint+Prettier规范React+Typescript项目](https://zhuanlan.zhihu.com/p/62401626) 
- [前端 CHANGELOG 生成指南](https://godbasin.github.io/2019/11/10/change-log/)