## 看影片學 Lua 程式設計

Lua 的語法很簡單，執行環境也很簡單，如果您用的是 Linux，應該從 [Lua 官網上下載](http://www.lua.org/download.html) 建置一下就可以了，以下是官網所提供的建置方法：

```
curl -R -O http://www.lua.org/ftp/lua-5.2.3.tar.gz
tar zxf lua-5.2.3.tar.gz
cd lua-5.2.3
make linux test
```

如果您用 MS. Windows ，那麼就可以安裝 Lua for Windows，以下是其網址：

* <http://luaforwindows.luaforge.net/>

下載安裝後，您會發現在「開始/所有程式」裏有個 Lua 的資料夾，裏面有「iLua, Lua Command Line, Lua Examples, QuickLuaTour」等項目，建議您看看「QuickLuaTour」，它會帶領你快速的熟悉 Lua 的語法與範例。

接著您可以直接起動命令列，然後用任何的編輯器，像是「Notepad++」等，開始寫一些簡單的程式，然後直接用 `lua <程式名稱>` 去執行您的程式即可。以下是筆者執行幾個 Lua 程式的過程：

```
D:\Dropbox\Public\pmag\201402\code>lua hello.lua
Hello World!

D:\Dropbox\Public\pmag\201402\code>lua fact.lua
factorial(5)=120

D:\Dropbox\Public\pmag\201402\code>lua obj.lua
10,20
30,40
50,60

D:\Dropbox\Public\pmag\201402\code>lua obj.lua
point(10,20)
point(30,40)
point(50,60)
```

您可以以看看下列 Lua 的影片，以便瞭解 Lua 的程式寫法：

| 影片                                               | 連結                                     |
|----------------------------------------------------|------------------------------------------|
| Lua Tutorial #1: Introduction and Setup            | <http://youtu.be/dHURyRLMOK0>            |
| Lua Tutorial #2: Hello World                       | <http://youtu.be/aSxoOCn6Y4E>            |
| Lua Tutorial #3: Variables and User Input          | <http://youtu.be/ClThmOGuMi4>            |
| Lua Tutorial #4: Basic Mathematics                 | <http://youtu.be/jQ40M1DObl4>            |
| Lua Tutorial #5: If and Else                       | <http://youtu.be/vlJftHgeByg>            |

當然、多寫多看，應該是學習程式的不二法門。學程式與學習游泳一樣，只有下水開始扭動身體，才有機會真正學會游泳，也只有真正開始上機寫程式，才有可能真正學會寫程式。對於 Lua 、當然也是如此！

