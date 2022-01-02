`self` is the object which we are passing
```python
class Computer:
    def config(self):
        print("luchi")

obj1 = Computer()
obj2 = Computer()
Computer.config()
```

```python
class Computer:
    def __init__(self):
        print("luchi")
    def config(self):
        print("luchiiii")
obj1 = Computer()
obj2 = Computer()
```
OP : 
luchi
luchi

---
```python
class Computer:
    def __init__(self):
        print("luchi")
    def config(self):
        print("luchiiii")
# obj1 = Computer()
# obj2 = Computer()
Computer.config(Computer())
```
OP : luchi
luchiiii
