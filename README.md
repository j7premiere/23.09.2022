### Task 7 kyu

[Task link](https://www.codewars.com/kata/56606694ec01347ce800001b/)

Implement a function that accepts 3 integer values a, b, c. The function should return true if a triangle can be built with the sides of given length and false in any other case.

(In this case, all triangles must have surface greater than 0 to be accepted).

### My solution

```Java

class TriangleTester{
  public static boolean isTriangle(int a, int b, int c){
    if((a+b>c)&&(a+c>b)&&(b+c>a)){return true;}
    else {return false;}
    }
  }

```

### Favourite solution from code-wars

```Java

class TriangleTester
{
  public static boolean isTriangle(int a, int b, int c)
  {
    return (Math.max(Math.max(a,b),c) < (a+b+c-Math.max(Math.max(a,b),c)));
    //no side can be larger than the sum of the two other sides
  }
}

```

I like this solution because i find it interesting to use math functions

# Have a nice day!