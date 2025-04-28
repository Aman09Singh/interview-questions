### Problem Statement ::

Given an array arr[] of n integers, construct a product array res[] (of the same size) 
such that res[i] is equal to the product of all the elements of arr[] except arr[i]. 
Example: 
Input: arr[] = [10, 3, 5, 6, 2]
Output: [180, 600, 360, 300, 900]



```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {10,3,5,6,2};
        int[] res = new int[5];
        int mult = 1;
        for(int i=0;i<5;i++){
            for(int j=0;j<5;j++){
                if(i==j){
                    continue;
                }else{
                    mult = mult * arr[j];
                }
            }
            res[i] = mult;
            mult = 1;
        }

        for(int i=0;i<5;i++){
            System.out.println(res[i]);
        }
    }
}
```




