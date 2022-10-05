```.py
## IP Creator: write a program in OOP that creates a set of ip addresses given the subnet and a number n,if the number is more than the possible number of host show “error” 

class IP_Creater:
    def __init__(self,subnet : str,n: int):
        self.subnet = subnet
        self.n = n
    def get_host(self,subnet,n):
        answer = []
        key = ""
        if n > 9:
            print("Error")
        else:
            for i in range(n):
                for x in range(len(subnet)-1):
                    key += subnet[x]
                key += str(i)
                answer.append(key)
                key = ""
        return answer

test1 = IP_Creater("192.168.4.0",4)
print(test1.get_host("192.168.4.0",4))
test2 = IP_Creater(“10.10.1.0”, 500)
print(test2.get_host(“10.10.1.0”, 500))
test3 = IP_Creater(“10.10.1.250”, 7)
print(test3.get_host(“10.10.1.250”, 7))
```
