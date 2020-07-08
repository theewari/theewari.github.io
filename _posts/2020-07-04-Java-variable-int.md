---
layout: post
title:  "Integer Variable Type In Java"
date:   2020-07-04 23:06:45 +0300
categories: Java
---
To declare a whole number in java, use `int` as the keyword. We should assign  the name and volume to the `int`. That assigning called initialization. 

```java
package variables.Variables;

public class IntSample {

    public static void main(String[] args) {
	// write your code here

        int a = 4;
        int b = 3;

        System.out.println(a+b);
        System.out.println(a-b);
        System.out.println(a*b);
        System.out.println(a/b);

        long c = 2147483648L;

        System.out.println(c);
    }
}
```

The `int` can store 32 bits. From (-2 ^ 31) to (2 ^ 31)  -  1

The `int` can’t store long numbers. At that time you need `long` as the keyword. You should type `L` after the number.

`long`  can store 64 bits. From (-2 ^ 63) to (2 ^ 63) - 1

There are another two types in integer to store small numbers. Those keywords are `bit` and `short`.

`bit` can store 8 bits. From (-2 ^ 7) to (2 ^ 7) - 1

`short` can store 16 bits. From (-2 ^ 15) to (2 ^ 15) -1






