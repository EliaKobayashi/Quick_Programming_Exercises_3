## Time Trial: Create a program that produces the pattern below.

```.py
def TimeTrial():
    counter = 1
    for z in range(3):
        for row in range(5):
            for column in range(5):
                print(str(counter).center(5), end=" ")
                counter += 1
            print("")
        print("")

print(TimeTrial())
```
[](quiz60_pic1.png)
[](quiz60_pic2.png)
[](quiz60_pic3.png)
