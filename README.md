# python-3.7
New things in python3.7. 

## Using dataclass and properties inplace of namedtuples
```python
from dataclasses import dataclass

@dataclass
class Animal:
  name:str
  no_of_legs:int
  alive:bool = True

  def (self):
    return f'I am {self.name} and I am {self.age} years old.'

  @property
  def move_again(self):
      return f'My name is {self.name} and I am {self.age} years old. I am moving again'

shabri = Person("Shabri",19)
print(shabri.move())
print(shabri.move_again)
```
