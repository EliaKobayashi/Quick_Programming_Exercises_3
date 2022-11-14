### Using the function that produces the table of Truth for 3 inputs, add a column for the boolean equation

```.py
def quiz70():
    for i in range(8):
        if i % 2 == 0:
            C = 0
        else:
            C = 1
        if i == 2 or i == 3 or i == 6 or i == 7:
            B = 1
        else:
            B = 0
        if i < 4:
            A = 0
        else:
            A = 1
        if B == 1:
            B = 0
        elif B == 0:
            B = 1
        answer = (A*B) + (B) + (B *C)
        if answer > 1:
            answer = 1
        print(f"{answer}\n")

print(quiz70())
```
![](quiz70_pic1.png)
![](quiz70_pic2.png)
