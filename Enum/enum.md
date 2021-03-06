# **enum 来实现枚举类**

## **代码演示枚举**

```java


public class Enumeration03 {
    public static void main(String[] args) {
        System.out.println(Season0.SPRING);
        System.out.println(Season0.SUMMER);
        System.out.println(Season0.AUTUMN);
        System.out.println(Season0.WINTER);

    }
}

// 演示自定义枚举实现
enum Season0 {//类

    // 定义了四个对象, 固定.
    // public static final Season0 SPRING = new Season0("春天", "温暖");
    // public static final Season0 WINTER = new Season0("冬天", "寒冷");
    // public static final Season0 AUTUMN = new Season0("秋天", "凉爽");
    // public static final Season0 SUMMER = new Season0("夏天", "炎热");
    // 如果使用了enum 来实现枚举类
    // 1. 使用关键字 enum 替代 class
    // 2. public static final Season SPRING = new Season("春天", "温暖")
    //    直接使用SPRING("春天", "温暖") 解读 常量名(实参列表)
    // 3. 如果有多个常量(对象)， 使用 ,号间隔即可
    // 4. 如果使用enum 来实现枚举，要求将定义常量对象，写在前面
    // 5. 如果我们使用的是无参构造器，创建常量对象，则可以省略 ()
    SPRING("春天", "温暖"),
    SUMMER("夏天", "温暖"),
    AUTUMN("秋天", "温暖"),
    WINTER("冬天", "温暖");
    private final String name;
    private final String desc;

    private Season0(String name, String desc) {
        this.name = name;
        this.desc = desc;
    }

    public String getName() {
        return name;
    }

    public String getDesc() {
        return desc;
    }

    @Override
    public String toString() {
        return "Season0{" +
                "name='" + name + '\'' +
                ", desc='" + desc + '\'' +
                '}';
    }
}


```

```java

class Test {
    public void say() {
/**
* Description: <br/>
* @author: sun <br/>
* @date: 2022/3/11 10:49<br/>
* @param:[]<br/>
* @return:void
*/
    }
}

```

# 代码

# 代码回退测试
