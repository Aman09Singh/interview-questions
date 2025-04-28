## Problem Statement ::

Find the 2nd largest element from the given array 

#### Solution ::

```java
public class Main {
    public static void main(String[] args) {
        int[] arr = {10,3,5,6,2};
        int[] res = Arrays.stream(arr).sorted().toArray();
        System.out.print("Second largest value from the array  :: " + res[arr.length-2]);
    }
}
```


