 实验四 字符串实验

实验目的

掌握字符串String及其方法的使用

掌握异常处理结构

业务要求

内容：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：

1.每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”

2.允许提供输入参数，统计古诗中某个字或词出现的次数

3.考虑操作中可能出现的异常，在程序中设计异常处理程序

输入：

汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>

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

过程：

创建名为Changhenge的class文件。

首先在Changhenge中输入长恨歌诗句的汉字字符串，并设置for循环语句，当汉字字数满足规定长度时，则按顺序输出一组字符。再设置判断语句，当字符串个数满足7的倍数并且除二余数为1时，则输出该字符串，并在字符串末尾添加“，”；当字符串个满足7的倍数并且为2的倍数时，则输出该字符串，并在字符串末尾添加“。”。

统计汉字“一”的个数，设置初始值count为0，从“一”的个数为-1时开始计算，每增加一个“一”字符，则count的值将会陆续加1。最后输出count的值即为字符“一”出现的次数。

使用try-catch监视try中的语句，如果代码区有错误，则将错误异常输出来。

核心代码：中的语句

//异常处理
				
try{

catch(Exception e){//

System.err.println("发生异常："+e.toString());

e.printStackTrace();
}
			
countString(str,"一");
 }
		       
//统计“一”的字数

private static void countString(String str, String string) {

// TODO Auto-generated method stub
				
int count=0;
				
while(str.indexOf(string)!=-1){
				
str=str.substring(str.indexOf(string)+1, str.length());
			
count++;
}
				
System.out.print(string+"出现的次数为："+count);
				
				
//判断语句

if((i+1)%7==0&&(i+1)%2==1||(i+1)%14==0&&(i+1)%2==0){

if((i+1)%7==0&&(i+1)%2==1)
					
bs.append(",");
					
else
				    
bs.append("。\n");
				    				    
//string字符串

public static void main (String[] args) {	

String str="汉皇重色思倾国御宇多年求不得杨.......";

for(int i=0;i<c.length;i++){

bs.append(c[i]);
				
System.out.print(bs.toString()); 

注释：

try{

catch(Exception e){  异常捕获
 
StringBuffer  字符串变量

编程感想：

通过这次实验，我掌握了string字符串及其方法的使用，学会了使用for循环语句和if判断语句将长段的汉字字符串分组的方法，了解了异常处理的使用，懂得了如何统计字符串中单个字符的数量，通过查询资料使我对流式布局和跳转有了更深刻的了解。通过这次课程实验，我懂得了基础同样也很重要，基础学好了才能学习更深入的东西。同时，我也认识到了很多自己的不足之处，也应该多虚心向同学请教，多查阅书记，这样才能不断进步。
