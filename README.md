#定义类（class）
#1.封装
class Shape:
    def __init__(self,name):#设置属性，构造函数(__init__),在创建对象时自动调用，用于初化属性
        self.name=name      #都是公开属性
    def area(self):
        pass

#2.继承
class S(Shape):#继承自上面的Shape
    def __init__(self,lengh):
        super().__init__("正方形")#调用父类函数
        self.lengh=lengh
    def area(self):
        print(f"正方形的面积是{self.lengh*self.lengh}")#3.多态-重写父类方法

class C(Shape):
    def __init__(self,banjing):
        super().__init__("圆形")#调用父类函数
        self.banjing=banjing
    def area(self):
        print(f"圆形的半径是{self.banjing*3.14}")

class T(Shape):
    def __init__(self,height,base):
        super().__init__("三角形")#调用父类函数
        self.height=height
        self.base=base
    def area(self):
        print(f"三角形的面积是{(self.height*self.base)/2}")

#使用类来创建对象
s=S(4)
c=C(4)
t=T(4,8)
#调用对象的属性和方法
#输出
s.name
s.area()
c.name
c.area()
t.name
t.area()
