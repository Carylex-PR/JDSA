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

