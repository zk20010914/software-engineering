# software-engineering
<**>public class TestMaoPao {
     
     public static void sortBub(int [] arr) {
             //总的交换次数
            int count =0;
            //遍历数组的趟数
            for( int i =0; i< arr. length-1; i++) {
                 for( int j =0; j< arr. length- i-1; j++) {
                //比较前一个元素与后一个元素的大小，将每趟中最大的元素放在末尾，
               // 末尾的元素再下一趟  不用再比较，所以 是  j< arr. length- i-1
                    //交换前后两个元素的位置
                      if( arr[ j]> arr[ j+1]) {
                            int temp = arr[ j];
                            arr[ j]= arr[ j+1];
                            arr[ j+1]= temp;
                            count++;
                     }
                }
           }
           System. out.println( "交换次数"+count );
     }
     
     public static void main(String[] args) {
           
            int [] arr = {2,23,1,34,23,45,12};
            sortBub(arr);
            for( int i=0; i< arr. length; i++) {
                System. out.print( arr[ i]+ " ");
           }
     }
}<**>
