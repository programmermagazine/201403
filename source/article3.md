## 根號求解 (作者：Bridan)

可能有人會好奇，計算機如何求得開根號數值，這裡提供個人所知的兩種方法。

**方法一：** [長除式演算法](http://zh.wikipedia.org/w/index.php?title=%E5%B9%B3%E6%96%B9%E6%A0%B9&variant=zh-tw)，可直接筆算求平方根值。

運用 (a + b)2- (2a + b) b = a2，初值 a = 0，反覆求 a 的後一位數值 b 。

例 Square(152.276)

```
  1  2. 3  4
 ------------   列式時以小數點為基準，兩位兩位一組。
/ 1 52.27 60    (2a + b) b
  1           = (2 x 0 + 1) x 1 , a = 0
 ------------
    52
    44        = (2 x 10 + 2) x 2 , a = 10
 ------------
     8 27
     7 29     = (2 x 120 + 3) x 3 , a = 120
 ------------
       98 60
       98 56  = (2 x 1230 + 4) x 4 , a = 1230
 ------------
           6
```
　

**方法二：** 以 [牛頓迭代法](http://zh.wikipedia.org/w/index.php?title=%E5%B9%B3%E6%96%B9%E6%A0%B9&variant=zh-tw) 計算求解

```
X = A1/N，將 A 開 N 次方根，

Xn+1 = [(N-1)Xn + A/XnN-1]/N ，(N＞0)

N = 2 時 ，A＞1，1＜Xn＜A
Xn+1 = [Xn + A/Xn]/2 ，(挑選適當的 Xn 初值可以快速收斂，只要計算兩三次就可得到正確數值)
```

其原理為，

```
X = [X + A/X]/2
2X = X + A/X
2X2 = X2 + A
X2 = A
X = A1/2
```

這方法是我從 [Engineering Formulas](http://www.anobii.com/books/01e14970c407f6b3a5/) 這本書學到的，此書為 *Reiner Gieck, Kurt Gieck* 合著 McGraw-Hill 出版 ISBN 9780070234550，它是我在公司文管中心發現的寶藏。

在網際網路尚未發達前，這類工具書對工程師是非常重要的，尤其需要常常查工程或數學公式很有用。

(本文來自「研發養成所」 Bridan 的網誌，原文網址為 <http://4rdp.blogspot.tw/2008/04/blog-post_9406.html> ，由陳鍾誠編輯後納入程式人雜誌)

