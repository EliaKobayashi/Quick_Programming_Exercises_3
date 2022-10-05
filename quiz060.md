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
1[](quiz60_pic.png)
