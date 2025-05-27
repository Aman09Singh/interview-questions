# Apptware Coding Questions Round 1

## Question 1 - Given a list of integers, find the second highest in O(n) time complexity

### Note: below code has to be factored.  

```java
//complexity and other methods of doing the same
////list of integers
////second highest number
//List<Integer> list = new ArrayList<>();
//        list.add(89);
//        list.add(12);list.add(45);list.add(56);list.add(23);
////disticnt to handle
//        for(int a : list){
//int largest = 0;
//int secondLargest = 0;
//
//        }
//Object[] arr = list.stream().distinct().sorted().toArray();
//        System.out.println(arr[arr.length-2]);
//        }
```

## Questions 2 - Given the classes, what would be the output of the following code when b.methodA(); is called 

```java
class A {

	public void methodA(){
	Sysout("In class A methodA");
	}
}

class B extends A{

	public void methodA(){
	Sysout("In class B methodA");
	}
}

class C {

	B b = new A();
	b.methodA();

}
```