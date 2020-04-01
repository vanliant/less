# less
less学习



- #### vsCode中设置easy-less

  - ##### setting.json中设置

    ```javascript
    "less.compile": {
            "compress": false, // true => remove surplus whitespace
            "sourceMap": false, // true => generate source maps (.css.map files)
            "out": "../css/", // false => DON'T output .css files (overridable per-file, see below)
    }
    ```

- #### less中的注释

  - ##### //不会编译为css

  - ##### /**/会编译到css中

- #### less中的变量

  - ##### 使用@来声明变量(例如： @pink：pink)

    - ###### 作为普通属性来使用，直接使用 @pink

    - ###### 作为选择器和属性名，#@{selector的值}的形式

    - ###### 作为url:@{url}

    - ###### 变量的延迟加载

- #### less中的嵌套规则

  - ##### 基本嵌套规则

  - ##### &的使用

    - ###### 代表平级关系

- #### less中的混合

  - ##### 混合就是将一系列的属性从一个规则集引入到另一个规则集的方式

    - ###### 普通混合,会造成css面积大

    - ###### 不带输出的混合，即加上（），（）中没有参数

    - ###### 带参数的混合

    - ###### 带默认值的混合