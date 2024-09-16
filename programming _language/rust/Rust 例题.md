# Rust 例子

# 1. Hello World

每门语言的开头菜——Hello，world

```rust
fn main(){
    println!("Hello World");
}
```

和很多语言一样，定义一个main函数，然后输出Hello，world。

和其他语言不同的是，rust的main前面接的返回值类型不是int，而是一个fn的关键字，这倒增添了不少神秘感。

我们打开命令行，运行我们编写的代码：

![image-20240915173032067](C:\Users\16920\AppData\Roaming\Typora\typora-user-images\image-20240915173032067.png)

与其他语言不一样的是，rust的输出不是常规的print或printf，而是println带了一个！，说实话，输出语句带一个！确实少见。官方给出的解释是：`println!` 是一个[**宏**](https://rustwiki.org/zh-CN/rust-by-example/macros.html)（macros），可以将文本输出到控制台（console）。宏目前还不知道它的概念，需要我深入学习了。

## 1.1 注释

和其他语言差不多，rust的注释：

- 普通注释，其内容将被编译器忽略掉：
  - `// 单行注释，注释内容直到行尾。`
  - `/* 块注释，注释内容一直到结束分隔符。 */`
- 文档注释，其内容将被解析成 HTML 帮助文档：
  - `/// 为接下来的项生成帮助文档。`
  - `//! 为注释所属于的项（译注：如 crate、模块或函数）生成帮助文档。`



## 1.2 格式化输出（待完成）



# 2. 原生类型

接触Rust，我一直觉得Rust的变量非常特别。我们先来看rust官方给出的标量类型：

> - 有符号整数（signed integers）：`i8`、`i16`、`i32`、`i64`、`i128` 和 `isize`（指针宽度）
> - 无符号整数（unsigned integers）： `u8`、`u16`、`u32`、`u64`、`u128` 和 `usize`（指针宽度）
> - 浮点数（floating point）： `f32`、`f64`
> - `char`（字符）：单个 Unicode 字符，如 `'a'`，`'α'` 和 `'∞'`（每个都是 4 字节）
> - `bool`（布尔型）：只能是 `true` 或 `false`
> - 单元类型（unit type）：`()`。其唯一可能的值就是 `()` 这个空元组

还有符复合类型：

> - 数组（array）：如 `[1, 2, 3]`
> - 元组（tuple）：如 `(1, true)`

我们跟着官方的练习敲一遍代码：

```rust
fn main(){
    let _logical: bool = true;

    let _a_float = 1.0;
    let _an_integer = 5i32;

    let mut _change_value = 2;
    _change_value = 30;

    let _change_value = true;
}
```

以上代码我简化了官方示例代码，但保留了核心部分，接下来我谈谈Rust类型与定义变量给我的感觉：

1. rust是静态的，所以定义变量肯定要声明变量类型，但是代码中都是let开头，声明的类型在变量名后面，同时还可以自动识别，也就是一开始声明变量不用指定类型，只要指定变量的目标数据，rust自动给你配置。
2. 使用别的语言编程，变量生成之后，我们可以让变量随意赋予新值（同类型的），但是rust不行，rust的变量赋值之后就固定了，要使用可变变量，需要加上mut，非常有意思，可能正因为如此，Rust才被赋予了安全性。
3. rust建议我们定义变量以_开头，不然就会警告。

## 2.1 元组

