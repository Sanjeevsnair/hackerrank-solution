# Here is my HackerRank Solutions
---
## 1.Lonely Integer
  - [Problem](https://www.hackerrank.com/challenges/lonely-integer/problem?isFullScreen=true)
  - [Solution](Grading_Students/gradingstudents.py)  
  - Explanation:
  > The problem is to find the lonely integer in an array, where all other elements appear twice. The XOR operator (^) is a key insight for solving this problem. The XOR of a number with itself is 0, so when you XOR all the elements in the array, the elements that appear twice will cancel each other out, leaving you with the lonely integer.
```python

def lonelyinteger(a):
    res = 0
    for elem in a:
        res ^= elem
    return res

print(lonelyinteger(a))


```

Define lonelyinteger using XOR to find the lonely integer in an array.
Read the length of the array (n) and the array (a) from the input.
Call lonelyinteger to find the lonely integer.
Write the result to the output file.

```
input:

5
0 0 1 2 1

Output:

2
```
In this example, we entered 3 grades: 73, 67, and 41. The first grade, 73, is rounded up to 75 because the remainder of 73 divided by 5 is 3, which is greater than or equal to 3. The second grade, 67, remains the same because the remainder of 67 divided by 5 is 2, which is less than 3. The third grade, 41, also remains the same because it is less than 38.
****
## 2.Flipping bits

  - [Problem](https://www.hackerrank.com/challenges/flipping-bits/problem?isFullScreen=true)
  - [Solution](Mini-Max_Sum/minimaxsum.py) (navigate to the Solution file)
  - Explanation:
  >The script seems to be performing a bitwise operation on each input number num. The expression ~num + correct involves taking the bitwise complement of num (flipping all its bits) and then adding a value represented by correct. The use of 1 << 32 suggests that it's working with 32-bit integers

```python
    correct = 1 << 32

    for _ in range(T):
        num = int(input().strip())
        print(~num + correct)

```
Read the number of test cases (T).
Set correct to represent the maximum unsigned 32-bit integer.
#### For each test case:
Read an integer num.
Print the result of ~num + correct, a bitwise operation.

#### Sample input & output
input
```
2
4
123456
```
output
```
4294967291
4294843839
```
****
## 3.CamelCase

  - [Problem](https://www.hackerrank.com/challenges/camelcase/problem?isFullScreen=true)
  - [Solution](Mini-Max_Sum/minimaxsum.py) (navigate to the Solution file)
  - Explanation:
  >The problem is to count the number of words in a camelCase string. In camelCase, words are concatenated, and each word (except the first) starts with an uppercase letter. The script counts the number of uppercase letters to determine the number of words.

```python
 def camelcase(s):
    res = 1
    for let in s:
        if let.isupper():
            res += 1

    if not s:
        res = 0

    return res

```
Checks if the script is run as the main program.
Reads a string s from the input, assuming it's a camelCase string.
Calls the camelcase function with the input string.
Prints the result, which is the count of words in the camelCase string.

#### Sample input & output
input
```
saveChangesInTheEditor


```
output
```
5


```
****


