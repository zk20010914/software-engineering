
# software-engineering

<**>冒泡排序的原理及实现！

<**>较相邻的元素。如果第一个比第二个大，就交换他们两个。 
对每一对相邻元素做同样的工作，从开始第一对到结尾的最后一对。在这一点，最后的元素应该会是最大的数。 
针对所有的元素重复以上的步骤，除了最后一个。
持续每次对越来越少的元素重复上面的步骤，直到没有任何一对数字需要比较。

白盒测试冒泡排序

public class BubbleSort {   
public void BubbleSort(int[] arr){  
for(int i=0;i<arr.length-1;i++){//外层循环控制排序趟数  
for(int j=0;j<arr.length-1-i;j++){//内层循环控制每一趟排序多少次
  
  if(arr[j]>arr[j+1]);
    int temp=arr[j];
　　　　　　　　    
            arr[j]=arr[j+1];
　　　　　　　　 　  
            arr[j+1]=temp;
　　　　　　　 }
        }
　　
        //输出
  
   
   System.out.println("排序后数组元素为:");
          for(int num : arr){
   
   System.out.print( num + "  " );
      }}　　
 
 3.测试用例
                   
                   语句覆盖 :  1.arr = {4,3,2,1}

                  判定覆盖 :  1.arr = {1,2,3,4};  2. arr = {4,3,2,1}

                  条件覆盖 :  1.arr = {1,2,3,4};  2. arr = {4,3,2,1}

                  路径覆盖 :  1.arr = {1,2,3,4};  2. arr = {4,3,2,1}
**


