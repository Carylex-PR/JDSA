- Time Complexity
- Space complexity


Loop from 1 to 7
- Best Case -> 1 -> Omega
- Average Case -> 4 -> Theta
- Worst Case -> 7 -> Big O

We always try to measure worst case

O(n)
```run-java
public class Main {
    public static void main(String args[]) {
        int n = 10;
        logItems(n);
    }
    
    public static void logItems(int n) {
        for (int i = 0; i < n; i++) {
            System.out.println(i);
        }
    }
}
```
```desmos-graph
y=x | label: y = x 
y = 5x | label: y = 5x 
```


- We drop constants of for Big O -> Why? -> Generalization and simplicity; However, remember a constant does effect time complexity, we are just avoiding it here.

O(1)
```run-java
public class Main {
	public static void main(String args[]) {
		int n = 5;
		n = oOf1(n);
		System.out.println(n);
	}

	public static int oOf1(int n) {
		return n+n+n;
	}
}
```


Different Terms for Inputs

O(2n)
```run-java
public class Main {
	public static void main(String args[]) {
		int n = 5;
		logItems(n);
	}

	public static void logItems(int n) {
		for (int i = 0; i < n; i++) {
			System.out.println(i);
		}
	
		for (int j = 0;j < n; j++) {
			System.out.println(j);
		}
	}
}
```

- If input n is replaced with 2 variables a,b -> it is O(a) + O(b) = O(a + b)
		If a nested a,b -> O(a * b)


Arrays
- Push and pop are O(1)
- Middle insert or delete needs to shift indexes -> O(n)
- Search by Value -> O(n)
- Search by Index -> O(1)

Wrap Up
- O(n^2) -> Loop within a Loop
- O(n)  -> Proportional
- O(log n) -> Divide and conquer
- O(1) -> Constant

![[Pasted image 20240223113514.png]]

**For Sorting Numbers**
![[Pasted image 20240223113612.png]]


