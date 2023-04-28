```
import java.util.Scanner;
//或者直接导入下面两个包
import java.util.*;
import java.io.*;
```
```
Scanner sc = new Scanner(System.in);
//读一个整数
int n = sc.nextInt();
//读一个字符串,遇到分号则输入终止
String s = sc.next();
//读一个浮点数
double t = sc.nextDouble();
//读一整行,中间可以有多个空格
String s = sc.nextLine(); 
```
```
System.out.print(n);//不换行输出
System.out.println(n);
```
**判断是否还有下一个输入**
```
sc.hasNext()
sc.hasNextInt()
sc.hasNextDouble()
sc.hasNextLine() 
```
**输出**
```
System.out.print(); 
System.out.println(); 
System.out.format();
System.out.printf();
格式化输出
double f = 111231.5585;
 // 保留 2 位小数（有四舍五入）
System.out.println(String.format("%.2f", f));
```


**2. 输入一个矩阵**
```
import java.util.Scanner;
public class Class_2 {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        int m = reader.nextInt();
        int n = reader.nextInt() ;
        int [][] array = new int[m][n] ;
        for (int i=0 ; i<m ; i++)
            for(int j=0 ;j<n ;j++)
            {
                array[i][j]=reader.nextInt();
            }
        reader.close() ;
        // 对矩阵按行打出
        for (int i=0 ; i<m ; i++)
        {
            for(int j=0 ;j<n ;j++)
            {
                System.out.print(array[i][j]+" ");
            }
            System.out.println( );
        }            
    }
}
```
**3. 输入一个单词字符串**
```
import java.util.Scanner;
public class Class_3 {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        String c = in.next() ;
        System.out.println(c);
        in.close();
    }
}

**你知道有几行输入**
Scanner in = new Scanner(System.in);
int n =in.nextInt();//n表示下面的输入行数
ArrayList<String> arr = new ArrayList<>();
While(n-- > 0){
  arr.add(in.next());
}
```
