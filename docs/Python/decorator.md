### Property
:::success
用來轉換class中的物件屬性  
使得private attribute可以用較直接的方式存取的同時，又可以不被任意修改
:::

#### Example

```python=
class Staff(object):
    def __init__(self, Name):
        self._Name = Name
```
* 當我們設計一個class的屬性時，因為要保護他不被任意修改，所以會希望讓他是private的，只有我們允許的對象才能修改和讀取。
* 最trivial的設計方式是如以下，加入get和set function
```python=
class Staff(object):
    def __init__(self, Name):
        self._Name = Name
    
    def get_Name(self):
        return self._Name
    
    def set_Name(self, new_Name):
        self._Name = new_Name
```
* 如此一來，我們便允許了"get_Name"和"set_Name"對"self.\_Name"進行修改
* 但是每次都要用一個function來改變值，而不是用"assignment symbol"(就是等號啦)來指派，難免有些不直觀
* 於是Property就登場了！
```python=
class Staff(object):
    def __init__(self, Name):
        self._Name = Name
    
    @property
    def Name(self):
        return self._Name
    
    @Name.setter
    def set_Name(self, new_Name):
        self._Name = new_Name

P = Staff("Jason")
print(P.Name)
P.Name = "Paul"
```
* 如以上的寫法，我們就可以直接print class object內的attribute
* 以及可以直接用"="來修改值
:::info
我們可以在class內的setter中進行判斷，以限制被輸入的數值類型
例如今天在第15行的地方輸入的不是string，而是int，則這個修改就可以在setter被擋下來
:::