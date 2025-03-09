# Calculator

#using calculator in python
class calculator:
  def __init__(self,a,b):
    self.a=a
    self.b=b
  def add(self):
    return self.a+self.b
  def sub(self):
    return self.a-self.b
  def mul(self):
    return self.a*self.b
  def div(self):
    return self.a/self.b
  def mod(self):
    return self.a%self.b
  def power(self):
    return self.a**self.b
  def squareroot(self):
    return (self.a**0.5,self.b**0.5)
  def cuberoot(self):
    return (self.a**1/3,self.b**1/3)
  def log(self):
    import math
    return (math.log(self.a), math.log(self.b))

a=int(input("enter the first number:"))
b=int(input("enter the second number:"))
obj=calculator(a,b)
print("1.Addition")
print("2.Subraction")
print("3.Multiplication")
print("4.Division")
print("5.Modulus")
print("6.Power")
print("7.Square Root")
print("8.Cube Root")
print("9.Logarithm")
print("10.Exit")
option=int(input("enter the option:"))
if option==1:
  print(obj.add())
elif option==2:
  print(obj.sub())
elif option==3:
  print(obj.mul())
elif option==4:
  print(obj.div())
elif option==5:
  print(obj.mod())
elif option==6:
  print(obj.power())
elif option==7:
  print(obj.squareroot())
elif option==8:
  print(obj.cuberoot())
elif option==9:
  print(obj.log())
