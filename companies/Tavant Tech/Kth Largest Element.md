# Largest element K at any point in the array.

If the value is not present, print -1 and if present print the value.  

```java
import java.util.Arrays;

public class Main {

    public static void KthLargestElement(int K, int N, int[] arr){
        for(int i=0,j=0;i<N;i++){
            int[] subArray  = Arrays.copyOfRange(arr,j,i+1);
            if(i+1 - K <= -1){
                System.out.println(-1 + " No value ");
            }else{
                int[] sortedArr = Arrays.stream(subArray).sorted().toArray();
                System.out.println(sortedArr[i+1-K] + " Value found ");
            }
        }
    }

    public static void main(String[] args) {
            int[] arr = {20,32,345,1,5};
            KthLargestElement(2,5,arr);
        }
    }

```