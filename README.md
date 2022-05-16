# Bits & Logic operations

### &&, || and !:
    !0x41 -> 0x00
    !0x00 -> 0x01
    !!0x41 -> 0x01
    
    0x69 && 0x51 -> 0x01 (return a number 1)
    0x69 || 0x51 -> 0x01
    
    P && *P (判断是否为空指针)
      
### .equals() 和 == 的使用情景：
    a. 当数据类型为基本类型时， 可以用==
    b. 当数据类型为引用数据类型时，用.equals()
    
### .equals()的原理：
    将此变量下的所有data和另一比较对象的所有data一一比较
    
### 字符串常量池
     public static void main(String[] args){
        String str = "Hello World";
        String str1 = "Hello World";
        
        //创建字符串常量时，JVM会检查字符串常量池中是否存在这个字符串
        //若字符串常量池中存在该字符串，则直接返回引用实例；若不存在，先实例化该字符串
        System.out.println (str==str1);// false

        String str2 = new String ("Hello World");
        System.out.println (str==str2);// false
    }

### Integer和int的比较
    


