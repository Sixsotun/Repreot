# Repreot// рекурсивная реализация Factorial
import java.util.Scanner;
class RecursiveFactorial
{
 public static void main(String[] args)
 {
  Scanner input=new Scanner(System.in);
  System.out.print("Find the Factorial of: ");
  int num=input.nextInt();
  System.out.println("Factorial of "+num+" = "+fact(num));
 }
static long fact(int n)
 {
  if(n < 2) return 1;
  return n * fact(n-1);
 }
}
from functools import reduce


Array.prototype.likeFilter = function (f) {
  let re = []
  this.forEach((e) => {
    if (f(e)) {
      re.push(e)
    }
  })
  return re
}

const arr = [1, 2, 3, 4, 5, 6]

console.log(arr.likeFilter((value) => value % 2 == 0)) // [2, 4, 6]
