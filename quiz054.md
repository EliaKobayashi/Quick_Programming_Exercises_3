```.py
class converter:
    def __init__(self, number):
        self.number = number

    def binirize(self):
        output = []
        output2 = []
        while self.number != 0:
            output.append(self.number % 2)
            self.number = self.number // 2
        while len(output) < 8:
            output.append(0)
        for i in range(8):
            output2.append(output[i])
        return output2

print(converter(number=10).binirize())
```
