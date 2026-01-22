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
```

#OUTPUT:
![EXP3(a) output](3(a)output.png)


#EXP-3B
#TOPIC:BinarySearch
```java
import java.util.Scanner;
import java.util.Arrays;

class BinarySearch {

    int list[];
    int size;
    int key = -1;

    BinarySearch(int size) {
        this.size = size;
        list = new int[size];
    }

    void set_list() {
        Scanner sc = new Scanner(System.in);
        for (int i = 0; i < list.length; i++) {
            list[i] = sc.nextInt();
        }
    }

    void get_list() {
        for (int i = 0; i < list.length; i++) {
            System.out.print(list[i] + " ");
        }
        System.out.println();
    }

    int binarysearch(int key) {
        int low = 0;
        int high = list.length - 1;

        while (low <= high) {
            int mid = (low + high) / 2;

            if (list[mid] == key) {
                return mid;
            } else if (list[mid] < key) {
                low = mid + 1;
            } else {
                high = mid - 1;
            }
        }
        return -1;
    }

    void getItem(int index) {
        System.out.println("Key element is found at index " + index);
        System.out.println("Key element is " + list[index]);
    }

   
}
import java.util.Scanner;
import java.util.Arrays;

 public class Bsearch{
 public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter size: ");
        int size = sc.nextInt();

        BinarySearch s = new BinarySearch(size);

        System.out.println("Enter elements:");
        s.set_list();

        Arrays.sort(s.list);  

        System.out.println("Sorted list:");
        s.get_list();

        System.out.print("Enter key to search: ");
        int key = sc.nextInt();

        int index = s.binarysearch(key);

        if (index != -1) {
             s.getItem(index);
        } else {
            System.out.println("Key element not found");
        }
    }
}
```

#output:
![exp3a output](3(b)output.png)



#EXP-3C
##TOPIC:BubbleSort
```java

import java.util.Scanner;
class Bubblesort{
    void Bsort(int arr[]){
          int n=arr.length;
           int temp = 0;
       for(int i=0;i<n-1;i++){
           for(int j=0;j<n-i-1;j++){
               if(arr[j]>arr[j+1]){
                    temp=arr[i];
                     arr[i]=arr[i+1];
                      arr[i+1]=temp;
}
}
}
}
}
import java.util.Scanner;

 public class Bubble{

     public static void main(String[] args){

           Scanner sc=new Scanner(System.in);

        System.out.println("Enter size of array:");

           int size=sc.nextInt();

           int[] integer=new int[size];

         for(int i=0;i<size;i++){

             System.out.println("Enter the value of integer at index"+i+":");

               integer[i]=sc.nextInt();

 }

    Bubblesort bs=new Bubblesort();

         bs.Bsort(integer);

      System.out.println("The sorted integer:");

     for(int i=0;i<size;i++){

         System.out.print(integer[i]+" ");
}
}
}
```

#output:
![exp 3c output](3(c)output.png)

