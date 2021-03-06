# 第七章\(反射\)

《《《 [返回首页](../../)  
《《《 [上一节](../di-liu-zhang-ju-ti-hua/6.10-jia-qi-lai.md)

## 反射

反射是一组功能的术语，它允许程序检查自己的定义。 `Java` 中的反射在类浏览器，对象检查器，调试器，解释器，服务（如 `JavaBeans™` 和对象序列化）以及任何创 建，检查或操作任意 `Java` 对象的工具中发挥作用。

`Java` 自一开始就出现了反射，但泛型的出现改变了反射的两种重要方式，即为泛型的反射和反射引入了泛型。

通过泛型来进行反射，我们指的是用于反射的一些类型现在是泛型类型。特别是，类 `Class` 成为泛型类 `Class<T>`。这看起来可能会让人感到困惑，但一旦明白它可以 使得使用反射的程序更加清晰。类文字和方法 `Object.getClass` 使用特殊技巧来返回更精确的类型信息。泛型被用来在注释的反映中特别有效。我们观察到 `Class<T>` 中的类型参数 `T` 应该总是绑定到一个可定义类型，并且我们提供一个简短的库，可以帮助您避免许多常见的未经检查的强制转换。

通过对泛型的反思，我们的意思是反射现在返回有关泛型的信息。有一些新的接口可以表示泛型类型，包括类型变量，参数化类型和通配符类型，还有一些新的方法可以获得 泛型类型的字段，构造函数和方法。

我们依次解释每一个点。我们不承担任何以前的反思知识，但我们专注于与泛型相关的方面。

我们依次解释每一个点。我们不承担任何以前的反思知识，但我们专注于与泛型相关的方面。

《《《 [下一节](7.1-fan-she-de-fan-xing.md)  
《《《 [返回首页](../../)

