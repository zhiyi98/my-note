  - ### 1.1 语法基础
    
    - #### 面向对象特性？
    
    ```
      // Java全栈知识体系 https://www.pdai.tech/md/java/basic/java-basic-oop.html
    
      //******************************************************************/
      // 问：谈谈你对面向对象的理解?
      //******************************************************************/
      // 答：
      //   我们都知道面向对象有三大特性，分别是封装、继承和多态。
      //   通常我们利用抽象数据类型和基于数据的操作封装在一起，构成一个实体类。数据被保存
      // 在这个对象内部，尽可能地隐藏内部的细节，只保留一个对外访问的接口与外部发生联系。
      // 用户无需知道对象内部的细节，当可以通过这个接口来访问该对象。
      //   子类继承了分类，从而获得了父类的非私有属性和方法，继承应该遵循里氏替换原则，子
      // 类对象必须替换到所有父类对象。
      //   多态分为运行时多态和编译时多态。编译时多态主要指方法的重载；运行时多态指对象的
      // 引用所直线的具体类型在运行时才能确定。运行时多态有三个条件：继承、重写和向上转型。
      //******************************************************************/
    
    
        public static class Instrument {
          public void play() {
            System.out.println("Instument is playing...");
          }
        }
    
        public static class Wind extends Instrument {
          public void play() {
            System.out.println("Wind is playing...");
          }
        }
    
        public static class Percussion extends Instrument {
          public void play() {
            System.out.println("Percussion is playing...");
          }
        }
    
        /**
         *
         * 著作权归https://pdai.tech所有。
         * 链接：https://www.pdai.tech/md/java/basic/java-basic-oop.html
         *
         *   下面的代码中，乐器类(Instrument)有两个子类: Wind 和 Percussion，它们都
         * 覆盖了父类的 play() 方法，并且在 main() 方法中使用父类 Instrument 来引用
         * Wind 和 Percussion 对象。在 Instrument 引用调用 play() 方法时，会执行实
         * 际引用对象所在类的 play() 方法，而不是 Instrument 类的方法。
         *
         */
        public static class Music {
          public static void main(String[] args) {
            List<Instrument> instruments = new ArrayList<>();
            instruments.add(new Wind());
            instruments.add(new Percussion());
            for(Instrument instrument : instruments) {
              instrument.play();
            }
          }
        }
    ```

    - #### a = a + b 与 a += b 的区别

    ```
    ```
    
    - #### 3*0.1 == 0.3 将会返回什么? true 还是 false?

    ```
    ```
    
    - #### 能在 Switch 中使用 String 吗?

    ```
    ```
    
    - #### 对equal()和hashCode()的理解?

    ```
    ```
    
    - #### final、finalize 和 finally 的不同之处?

    ```
    ```
    
    - #### String、StringBuffer与StringBuilder的区别？

    ```
    ```
    
    - #### 接口与抽象类的区别？

    ```
    ```
    
    - #### this() & super()在构造方法中的区别？

    ```
    ```
    
    - #### Java移位运算符？

    ```
    ```

参考：
[1] Java 全栈知识体系 https://www.pdai.tech/md/interview/x-interview.html#1-java-%E5%9F%BA%E7%A1%80