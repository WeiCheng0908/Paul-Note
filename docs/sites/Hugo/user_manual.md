
## Windows環境下

### 安裝GO
到[Go官網](https://go.dev/doc/install)下載穩定版本即可<br>
建議安裝於單純路徑，例如：C:\Go<br>
並且配置路徑於environment variable - %PATH%<br>

### 安裝Hugo
新增Hugo資料夾，底下包含bin，如下示意：<br>

```
└─Hugo
   └─bin
建議把Hugo放在單純路徑，例如：C:\Hugo\ 
```

到Hugo repo release下載穩定版本，放在Hugo\bin，並配置路徑於%PATH%<br>

#### 建立自己的新網站

`hugo new site <blog-name>`: 在本地資料夾產生一新網站資料集<br>
`git init`: 建立local git repo，以便後續主題安裝以及部屬於github page<br>

### 導入主題(以LoveIt為例)

!!! warning

    使用此主題必須安裝extended Hugo

`git submodule add https://github.com/dillonzq/LoveIt.git themes/LoveIt`: 使用git submodule安裝主題<br>


#### 配置config.toml