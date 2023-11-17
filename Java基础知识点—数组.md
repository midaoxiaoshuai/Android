# 基础知识点

![image-20231022200644475](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022200644475.png)

**类名**：对于所有的类来说，类名的首字母应该大写。如果类名由若干单词组成，那么每个单词的首字母应该大写，

**源文件名**：源文件名必须和类名相同。

**主方法入口**：所有的 Java 程序由 **public static void main(String[] args)** 方法开始执行。

![image-20231022202928513](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022202928513.png)

**String[] args 大写且空格**



### 编译，运行代码

![image-20231022201506178](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022201506178.png)

![image-20231022201817809](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022201817809.png)

![image-20231022203424563](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022203424563.png)

#### 案例常见错误

![image-20231022205004452](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022205004452.png)

一般这是默认勾选了的

![image-20231022205631050](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022205631050.png)

不勾选会隐藏文件扩展名



![image-20231022205421125](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022205421125.png)

![image-20231022205535048](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022205535048.png)

本质为文本而不是Java

![image-20231022220342585](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022220342585.png)

无*才是保存成功的



### 对象与类

![image-20231022223433235](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231022223433235.png)	`	![image-20231023164950441](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231023164950441.png)

![image-20231024145455082](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231024145455082.png)

### 修饰符

![image-20231024151047483](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231024151047483.png)

Java 程序的 main() 方法必须设置成公有的，否则，Java 解释器将不能运行该类。

![image-20231024155456498](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231024155456498.png)

### 加号的使用主要为连接符

![image-20231025211610010](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231025211610010.png)

### 关于设置和获取

#### 1：需要set方法和get方法（他们是一对）

![image-20231026174310426](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231026174310426.png)

#### 2.直接给他个内容



#### 强制类型转换

![image-20231029170822615](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029170822615.png)





#### 死循环

![image-20231029171537152](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029171537152.png)





#### 随机数

![image-20231029194415979](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029194415979.png)



![image-20231029200353339](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029200353339.png)



![image-20231029195707863](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029195707863.png)



这只能产生一个随机数

![image-20231029195757185](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029195757185.png)产生了20个随机数

![image-20231029200150323](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029200150323.png)

15是因为括号内的数应该比最大的数大1

#### scanner函数

在Java中，`Scanner` 是一个类，它位于 `java.util` 包中。`Scanner` 类提供了一种方便的方式来从用户输入、文件或其他输入源中获取各种类型的数据。

使用 `Scanner` 类，你可以读取用户在控制台输入的数据，例如整数、浮点数、字符串等。它提供了各种方法来解析和提取输入数据，并将其转换为适当的数据类型。

以下是使用 `Scanner` 类读取用户输入的示例：

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter your name: ");
        String name = scanner.nextLine();
```

        System.out.print("Enter your age: ");
        int age = scanner.nextInt();
    
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    
        scanner.close();
    }
}
```

在上面的示例中，我们首先创建了一个 `Scanner` 对象 `scanner`，并将其与标准输入流（`System.in`）关联。然后，我们使用 `nextLine()` 方法读取用户输入的名称，并使用 `nextInt()` 方法读取用户输入的年龄。最后，我们将读取到的数据打印到控制台上。

需要注意的是，在使用完 `Scanner` 对象后，应该调用 `close()` 方法来释放资源。

总而言之，`Scanner` 类提供了一种方便的方式来读取用户输入和其他输入源中的数据，并进行相应的数据类型转换。
```

java.util 包是 Java 标准库中的一个核心包，提供了许多常用的工具类和数据结构。以下是 java.util 包中一些常用类的概述：

Random：用于生成伪随机数的类。
Scanner：用于从输入源（例如控制台、文件）读取数据的类。
Arrays：提供了对数组进行操作的工具方法，例如排序、搜索等。
Collections：提供了对集合进行操作的工具方法，例如排序、搜索等。

在Java中，nextLine() 和 nextInt() 是 Scanner 类提供的两种不同的方法，用于从输入源读取不同类型的数据。

nextLine() 方法用于读取输入源中的一行文本，并将其作为字符串返回。它会读取输入直到遇到换行符（包括换行符），并将整行文本作为结果返回。这个方法通常用于读取包含空格的字符串或读取多个单词的输入。
下面是一个使用 nextLine() 方法的示例：

Scanner scanner = new Scanner(System.in);
System.out.print("Enter a sentence: ");
String sentence = scanner.nextLine();
System.out.println("You entered: " + sentence);
如果用户输入了 "Hello World"，那么 sentence 变量将包含字符串 "Hello World"。

nextInt() 方法用于读取输入源中的下一个整数，并将其作为整数返回。它会跳过任何前导空白符（如空格、制表符等），然后读取直到遇到非数字字符为止（包括非数字字符）。这个方法通常用于读取整数类型的输入



##### 猜数游戏

![image-20231029215010804](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029215010804.png)

#### length的使用区别

![image-20231029224038680](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029224038680.png)

数组的length是可以认为几个字符串几个字母（元素），字符串的length可以认为几个字母，而list(数组)的size也是元素个数



### 数组

#### 初始化

![image-20231029222055947](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231029222055947.png)

#### 输出数组

![image-20231030183411243](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030183411243.png)

![image-20231030183511598](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030183511598.png)

![image-20231030211730919](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030211730919.png)

![image-20231030214259508](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030214259508.png)

#### 多维数组初始化

![

](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030212005338.png)

a为数组名

![image-20231030212318974](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030212318974.png)

![image-20231030214406130](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030214406130.png)



#### java.util.Arrays 类能方便地操作数组，它提供的所有方法都是静态的

![image-20231030215911230](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231030215911230.png)

**public static int binarySearch(Object[] a, Object key)**

你提供的代码片段是一个公共静态方法的声明，该方法名为 `binarySearch`，接受两个参数：一个 `Object` 类型的数组 `a` 和一个 `Object` 类型的 `key`。

这个方法看起来是用于实现二分查找算法，用于在给定的数组中查找指定的关键字。二分查找算法是一种高效的查找算法，适用于已排序的数组。

要完整实现这个方法，你需要编写方法体来执行二分查找算法的逻辑。以下是一个示例实现：

```java
public static int binarySearch(Object[] a, Object key) {
    int low = 0;
    int high = a.length - 1;

    while (low <= high) {
        int mid = (low + high) >>> 1;
        Comparable midVal = (Comparable) a[mid];
        int cmp = midVal.compareTo(key);

        if (cmp < 0) {
            low = mid + 1;
        } else if (cmp > 0) {
            high = mid - 1;
        } else {
            return mid; // 找到了关键字，返回索引
        }
    }

    return -1; // 没有找到关键字，返回 -1
}
```

这个示例实现假设数组中的元素实现了 `Comparable` 接口，以便进行比较。你可以根据具体的需求和数据类型来修改和调整这个实现。

请注意，这只是一个示例实现，并不考虑所有的边界情况和错误处理。在实际使用中，你可能需要进一步完善和测试这个方法，以确保其正确性和鲁棒性。





public class Test {
    public static void main(String args[]) {
        String str = "helloworld";
        char[] data = str.**toCharArray**();// 将字符串转为数组
        for (int x = 0; x < data.length; x++) {
            System.out.print(data[x] + "  ");
            data[x] -= 32;
            System.out.print(data[x] + "  ");
        }
        System.out.println(new String(data));
    }
}

这段代码是一个简单的 Java 程序，它将字符串转换为字符数组，并将每个字符转换为大写形式后输出。

代码中的 main 方法是程序的入口点，它首先创建一个字符串 str 并赋值为 "helloworld"。然后，通过调用 toCharArray() 方法，将字符串转换为字符数组 data。

接下来，使用一个 for 循环遍历字符数组中的每个字符。在循环内部，首先使用 System.out.print() 方法输出当前字符，然后将该字符转换为大写形式，通过将其 ASCII 值减去 32 实现（假设当前字符是小写字母）。最后，再次使用 System.out.print() 方法输出转换后的字符。

循环结束后，使用 new String(data) 创建一个新的字符串对象，并通过 System.out.println() 方法输出该字符串。

**结果为**

h  H  e  E  l  L  l  L  o  O  w  W  o  O  r  R  l  L  d  D
HELLOWORLD





- 给数组赋值：通过fill方法。
-  对数组排序：通过sort方法,按升序。
-  比较数组：通过equals方法比较数组中元素值是否相等。

import java.util.Arrays;

public class **TestArrays {**
    public static void output(int[] array) {
        if (array != null) {
            for (int i = 0; i < array.length; i++) {
                System.out.print(array[i] + " ");
            }
        }
        System.out.println();
    }

    public static void main(String[] args) {
        int[] array = new int[5];
        // 填充数组
        Arrays.fill(array, 5);
        System.out.println("填充数组：Arrays.fill(array, 5)：");
        TestArrays.output(array);
        // 将数组的第2和第3个元素赋值为8
        Arrays.fill(array, 2, 4, 8);
        System.out.println("将数组的第2和第3个元素赋值为8：Arrays.fill(array, 2, 4, 8)：");
        TestArrays.output(array);
        int[] array1 = { 7, 8, 3, 2, 12, 6, 3, 5, 4 };
        // 对数组的第2个到第6个进行排序进行排序
        Arrays.sort(array1, 2, 7);
        System.out.println("对数组的第2个到第6个元素进行排序进行排序：Arrays.sort(array,2,7)：");
        TestArrays.output(array1);
        // 对整个数组进行排序
        Arrays.sort(array1);
        System.out.println("对整个数组进行排序：Arrays.sort(array1)：");
        TestArrays.output(array1);
        // 比较数组元素是否相等
        System.out.println("比较数组元素是否相等:Arrays.equals(array, array1):" + "\n" + Arrays.equals(array, array1));
        int[] array2 = array1.clone();
        System.out.println("克隆后数组元素是否相等:Arrays.equals(array1, array2):" + "\n" + Arrays.equals(array1, array2));
        // 使用二分搜索算法查找指定元素所在的下标（必须是排序好的，否则结果不正确）
        Arrays.sort(array1);
        System.out.println("元素3在array1中的位置：Arrays.binarySearch(array1, 3)：" + "\n" + Arrays.binarySearch(array1, 3));
        // 如果不存在就返回负数
        System.out.println("元素9在array1中的位置：Arrays.binarySearch(array1, 9)：" + "\n" + Arrays.binarySearch(array1, 9));
    }
}

 **int[] array2 = array1.clone();**



![image-20231101092331313](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231101092331313.png)

在 Java 中，可以使用 clone() 方法来复制一个数组。根据你的代码片段 int[] array2 = array1.clone();，它创建了一个数组 array2，并将 array1 的内容复制到 array2 中。

![image-20231101092318144](C:\Users\pingn\AppData\Roaming\Typora\typora-user-images\image-20231101092318144.png)