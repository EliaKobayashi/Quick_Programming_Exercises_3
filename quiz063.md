## There are N closed doors in a school and N students present. The first student opens each door. The second student flips (open⇆close) every second door. The third student flips every third door, and so on. 

Create a class that shows the doors open after N students. And the __repr__ shows the doors open in a colorful message


```.py
import random
from random import randint


class quiz65:
    def __init__(self,n):
        self.n=n
        self.answer = int

    def count(self):
        list = [False] * self.n
        for i in range(1, self.n + 1):
            for k in range(1, self.n + 1):
                if k % i == 0:
                    list[k - 1] = not list[k - 1]
        self.answer = sum(list)
        return self.answer

    def __repr__(self):
        colors = ["\033[1;41m", "\033[1;42m", "\033[1;43m", "\033[1;44m"]
        answer2 = ""
        answer2 += f"{colors[random.randint(1,3)]} {self.answer} \033[00m"
        return answer2

test1 = quiz65(100)
test2 = quiz65(10)
test3 = quiz65(200)
test4 = quiz65(5678)
print(test1.count())
print(test1)
print(test2.count())
print(test2)
print(test3.count())
print(test3)
print(test4.count())
print(test4)
```
![](quiz63.png)
