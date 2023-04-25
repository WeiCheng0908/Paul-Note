### 尋找git-for-windows下vimrc位置
* 開啟git bash
* 輸入 ```vim --version | grep vimrc```
就會返回vimrc存放的位置，如

```
   system vimrc file: "/etc/vimrc"
     user vimrc file: "$HOME/.vimrc"
 2nd user vimrc file: "~/.vim/vimrc"
```
!!! note

    1. 在git-for-windows裡，root directory就是..../git-for-windows
    2. 想知道$HOME在哪裡可以`echo %HOME%`出來看

建議修改 ==user vimrc file==，比較能做細節設定  

### vimrc設定