# 函数式编程

---

## lambda表达式 & 方法引用

- lambda
  - `() ->{}`
  - `(e) -> { return o; }`
- 方法引用
  - `Class::staticMethod`
  - `object::accessAllowedMethod`

## 函数式接口(PCBF)

`java.util.function`

### Function
- `Function<T, R>`

  change `T` to `R`

- `XXXFunction<R>`

  基本类型转换为`R`

- `ToXxxFunction<T>`

  `T`转换为基本类型

- `BiFunction<T, U, R>`

  `T`,`U` -> `R`

- `XxxToXxxFunction`

  基本类型转换

- `BinaryOperator<T>`

- `XXXBinaryOperator`

### Provider
- `Supplier<T>`
- `XxxSupplier`

### Consumer
- `Consumer<T>`
- `BiConsumer<T,U>`

### Predicate
- `Predicate`
- `BiPredicate`

### Thread
- `java.lang.Runnable`
- `java.util.concurrent.Callable`

### Compare
- `java.util.Comparator`

### File
- `java.io.FileFilter`
- `java.nio.file.PathMatcher`

### Proxy
- `java.lang.reflect.InvocationHandler`

### Java beans
- `java.beans.PropertyChangeListener`

### Other
- `java.security.PrivilegedAction`
- `java.awt.event.ActionListener`
- `javax.swing.event.ChangeListener`

## Stream

- `map`
- `flatMap`
- `filter`
- `peek`



- `sorted`
- `skip`
- `limit`
- `distinct`



- `foreach`
- `collector`
- `reduce`
- `find`



## Optional

- `ofNullable`
- `empty`



- `persent`
- `ifPersent`
- `map`
- `flatMap`
- `orElse`
- `orElseThrow`

