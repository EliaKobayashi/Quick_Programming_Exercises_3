'''.py
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

output = IP_Creater("192.168.4.0",4)
print(output.get_host("192.168.4.0",4))
'''
