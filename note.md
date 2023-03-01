1. 
    typeof 无法检查空值. 
    <!-- typeof null = object -->
    JS 的 Bug

2. 类型转换时 使用toString() 对于null 和 undefined 会报错. 使用String() 函数则不会报错.

3. 
    1. 如果字符串是合法的数字("3.14156"), 可以转换。
    2. 但是如果不是合法的数字 ("123abc"), 则不可以转换, NaN.
    3. 空字符串或者纯空格 转换为 0。
    4. null 转换为 0  undefined 转换为NaN.

4. parseInt(), parseFloat() 可以处理非全数字的文本转换('123px') => 123. 但是如果开头就不合法('a123') => 还是会转换成NaN.

> 需要注意 parseInt(123.45) => 123 因为小数点非有效数字.

5. 使用+ 号可以将 合法字符转换成数字 ("123")

    +"123" => 123


6. "12" < "2" => true; 字符比较Unicode这里 用 "12" 的 1 和 "2" 进行比较. 

7. null 和 undefined 返回 true. ** undefined 转换成数字时候转化成NaN。

8. NaN == NaN => false.  