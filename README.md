# javaExercises

## answers

1. Q: Why should you have minimum scope for variables? <br>
   A: 将局部变量的作用域最小化，可以增加代码的可读性和可维护性，并降低出错的可能性。<br>

2. Q: Why should you understand performance of String Concatenation? <br>
   A: +， Join，StringBuffer，StringBuilder，String.concat()几种拼接方式的开销不同<br>

3. Q: What are the best practices with Exception Handling? <br>
   A: 1、在 Finally 清理资源或者使用 Try-With-Resource 特性<br>
      2、优先明确异常<br>
      3. 记录你所指定的异常<br>
      4. 使用描述性消息抛出异常<br>
      5. 最先捕获特定的异常<br>
      6. 不要在catch中使用Throwable<br>
      7. 不要忽略Exceptions<br>
      8. 不要记录和抛出一个异常<br>
      9. 包装异常<br>

4. Q: When is it recommended to prefer Unchecked Exceptions? <br>
   A: 编译器不会检查这类异常，不检查的则开发者在代码的编辑编译阶段就不是必须处理，这类异常一般可以避免，因此一般是无需处理的。<br>

5. Q: When do you use a Marker Interface? <br>
   A: 标识接口是没有任何方法和属性的接口，它仅仅表明实现它的类属于一个特定的类型。当一个类实现了一个标识接口之后就像是给自己打了个标签。<br>

6. Q: Why are ENUMS important for Readable Code? <br>
   A: 枚举是类型安全的，不会出现取值范围错误的问题。同时，客户端不需要建立对枚举中常量值的了解，使用起来很方便，并且可以容易地对枚举进行修改，而无需修改客户端。<br>
      如果常量从枚举中被删除了，那么客户端将会失败并且将会收到一个错误消息。枚举中的常量名称可以被打印，因此可以获取更多信息。<br>

7. Q: Why should you minimize mutability? <br>
   A: 1.不可变类要比可变类更加易于设计，实现和使用。它们不容易出错，且更加安全。<br>
      2.不可变对象本质上是线程安全的，它们不要去同步。<br>
      3.不可变对象可以被自由地共享。<br>

8. Q: What is functional programming? <br>
   A: 函数式编程中没有赋值语句，因此变量一旦有了值就不会再改变。更通俗的讲，函数式编程没有副作用——除了结算结果，调用函数没有别的作用。<br>
      因为没有能够改变表达式值的副作用，可以在任何时候对它求值。由于能够在任何时候对表达式求职，所以可以用变量的值来自由替换表达式，反之亦然——即程序是“引用透明”的。<br>

9. Q: Why should you prefer Builder Pattern to build complex objects? <br>
   A: 1、需要生成的产品对象有复杂的内部结构，这些产品对象具备共性；<br>
      2、隔离复杂对象的创建和使用，并使得相同的创建过程可以创建不同的产品。<br>
      3、需要生成的对象内部属性本身相互依赖。<br>
      4、适合于一个具有较多的零件（属性）的产品（对象）的创建过程。<br>

10. Q: Why should you avoid floats for Calculations? <br>
    A:计算机是二进制的。浮点数没有办法是用二进制进行精确表示。<br>
      我们的CPU表示浮点数由两个部分组成：指数和尾数，这样的表示方法一般都会失去一定的精确度，有些浮点数运算也会产生一定的误差。<br>

11. Q: Why should you build the riskiest high priority features first?<br>
