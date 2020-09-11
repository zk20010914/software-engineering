# software-engineering

<**>冒泡排序的原理及实现
较相邻的元素。如果第一个比第二个大，就交换他们两个。 
对每一对相邻元素做同样的工作，从开始第一对到结尾的最后一对。在这一点，最后的元素应该会是最大的数。 
针对所有的元素重复以上的步骤，除了最后一个。
持续每次对越来越少的元素重复上面的步骤，直到没有任何一对数字需要比较。<**>

public class BubbleSort {
 
    public static void main(String[] args) {
        int [] arr = {49、38、65、97、76、13、27、49};
        bubbleSort(arr,arr.length);
    }
 
    public static void bubbleSort(int[] arr, int n) {
        for (int i=1,len=arr.length;i<len;i++){
           //标识符，判断这趟排序是否发生位置变化，没有发生，则排序已经完成，无须执行剩下循环
            Boolean flag=true;
            for (int j=1;j<len;j++){
                if (arr[j-1] > arr[j]){
                    int tmp = arr[j];
                    arr[j] = arr[j-1];
                    arr[j-1] = tmp;
                    flag=false;
                }
            }
            //排序过程打印记录
            System.out.println(Arrays.toString(arr));
            if (flag){
                 return ;
            }   
        }
    }
}
