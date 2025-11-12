# my-leiyuduixiang-project
class Shape:
    def __init__(self,name):
        self.name=name
    def area(self):
        pass
class S(Shape):
    def __init__(self,lengh):
        super().__init__("正方形")
        self.lengh=lengh
    def area(self):
        print(f"正方形的面积是{self.lengh*self.lengh}")
class C(Shape):
    def __init__(self,banjing):
        super().__init__("圆形")
        self.banjing=banjing
    def area(self):
        print(f"圆形的半径是{self.banjing*3.14}")
class T(Shape):
    def __init__(self,height,base):
        super().__init__("三角形")
        self.height=height
        self.base=base
    def area(self):
        print(f"三角形的面积是{(self.height*self.base)/2}")

s=S(4)
c=C(4)
t=T(4,8)
s.name
s.area()
c.name
c.area()
t.name
t.area()
