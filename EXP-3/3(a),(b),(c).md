#EXP-3(a)
##topic=constructor overloading
   
``` java
class Student{
     String name;
     int age;
     double marks;
  Student(String n,int a,double m){
       name=n;
       age=a;
       marks=m;
  }
  Student(){
 
 }
void display(){
System.out.println("Name:"+name);
System.out.println("Age:"+age);
System.out.println("Marks:"+marks);
}
}
public class Main{
    public static void main(String[] args){
          Student s1 = new Student();
          Student s2 = new Student("shilpa",19,85.5);
                 s1.display();
                 s2.display();
}
}
#OUTPUT:
![EXP3(a) output](Screenshot2026-01-22213721.png)
