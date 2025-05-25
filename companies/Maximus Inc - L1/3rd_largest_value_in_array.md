## Problem
 - Get the third largest value from the sorted Array

## Solution 

 - Sort the array
 - get the 4th element or you can do arr.length() - 2

```java
import java.util.Arrays;

public class Main{
    public static void main(String args[]){

        int[] arr = {23, 54, 78, 3, 8};
        int[] resultArr = Arrays.stream(arr).sorted().toArray();
        System.out.println(resultArr[3]);
    }
}
```


