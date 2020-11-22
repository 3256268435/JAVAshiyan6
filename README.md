# JAVAshiyan6
# 一、实验目的
  ### 1、掌握字符串String及其方法的使用
  ### 2、掌握文件的读取/写入方法
  ### 3、掌握异常处理结构

# 二、实验内容
  ## 在某课上,学生要提交实验结果，该结果存储在一个文本文件A中。
文件A包括两部分内容：
一是学生的基本信息；
二是学生处理后的作业信息，该作业的业务逻辑内容是：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能方法，实现如下功能：

每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
允许提供输入参数，统计古诗中某个字或词出现的次数
输入的文本来源于文本文件B读取，把处理好的结果写入到文本文件A
考虑操作中可能出现的异常，在程序中设计异常处理程序

输入：汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>

输出：
汉皇重色思倾国，御宇多年求不得。
杨家有女初长成，养在深闺人未识。
天生丽质难自弃，一朝选在君王侧。
回眸一笑百媚生，六宫粉黛无颜色。
春寒赐浴华清池，温泉水滑洗凝脂。
侍儿扶起娇无力，始是新承恩泽时。
云鬓花颜金步摇，芙蓉帐暖度春宵。
春宵苦短日高起，从此君王不早朝。
…………

                

# 三、实验要求
  ### 1、设计学生类（可利用之前的）
  ### 2、采用交互式方式实例化某学生
  ### 3、设计程序完成上述的业务逻辑处理，并且把“古诗处理后的输出”结果存储到学生基本信息所在的文本文件A中。

# 四、流程图

![结果](https://github.com/3256268435/Java-3/blob/main/%E6%B5%81%E7%A8%8B%E5%9B%BE.png)

# 五、核心方法
``` package thirdjava;

public class test {
    public static void main(String[] args) {
    	System.out.println("学生选课系统");
    	Student a = new Student(2019310629, "张三", "MALE");
        System.out.println("学生信息");
        System.out.println(a);
        Teacher d = new Teacher(01, "于春娜", "FEMALE", "大学物理", "资深教师");
        Teacher e = new Teacher(02, "张晓明", "MALE", "大数据导论", "教授");
        Teacher f = new Teacher(03, "金玲", "MALE", "金属工程", "普通教师");
        System.out.println("教师信息");
        System.out.println(d);
        System.out.println(e);
        System.out.println(f);
        Course g = new Course("大学物理", 01, "教207", 90f);
        Course h = new Course("大数据导论", 02, "综0915", 90f);
        Course i = new Course("金属工程", 03, "平方", 180f);
        System.out.println("课程信息");
        System.out.println(g); 
        System.out.println(h);
        System.out.println(i);
        a.tuike();
        a.delete();
        System.out.println("学生课程信息");
        System.out.println(a);
        Teacher x = new Teacher(02, "张晓明", "MALE", "大数据导论", "教授");
        Teacher y = new Teacher(03, "金玲", "MALE", "金属工程", "普通教师");
        System.out.println(x);
        System.out.println(y);
   
}
}   

```

# 六、实验结果

![结果](https://github.com/3256268435/Java-3/blob/main/%E7%BB%93%E6%9E%9C.png)

# 七、实验感想
通过这次实验学会了使用extend的继承方法，再利用super的方法来调用函数，super方法的使用进一步简化了程序，使程序变得不再复杂。同时也学会了toString的使用方法，public String toString()返回该对象的字符串表示。通常，ToString方法会返回一个“以文本方式表示”此对象的字符串。
