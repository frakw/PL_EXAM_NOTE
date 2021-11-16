# 程式語言期中考博物館
館長：貓咪大佬
管理員：JunYao、7How
開館日期：2021/11/15
免責聲明：本館展物僅用參考，若你的期中考因為本館所展示之答案考爆了，請找B10815044謝鈞曜索取賠償。
## 名詞解釋館
*	**Pascal**：
    * 一種imperative language
    * 一種命令式語言
    * ~~商用語言~~
*	**Overloaded operator**：給予operator多種意義、用途
*	**Subtype**：是Subclass，但沒有修改從Superclass繼承下來的method，稱為Subtype
*	**Garbage collection**：將散落的記憶體回收再利用
*	**Lifetime** : 變數從allocate到deallocate的時間
*	**Strong typing** : 
    *	執行前就需定義好變數型別的程式語言
    *	在執行前可以檢查出所有type error
    *	不容許隱性的型別轉換，在執行前會檢查出所有type error
*	**Polymorphism**(多態性)：override後仍使用相同名稱，但實作不同
*   Method overriding : 繼承superclass的method使用相同的名稱，但是內容不同
*	**Dynamic binding**：Runtime時，才會決定變數的型態
*	**Coercion**：強制改變type，又分：
    * Widening: 轉換後值不改變(int -> float) | Narrowing: 轉換後值會改變(float -> int)
*   **Von Neumann bottleneck**：CPU 和 Memory 之間的資料傳輸速度比 CPU 執行速度慢，因此資料傳輸速度決定了電腦的速度
*   **Von Neumann Architecture**：將程式指令記憶體和資料記憶體合併在一起的電腦設計概念架構
*   Static typing：在Compile time時就決定變數的type，且run time時無法被改變
*	Structure type compatibility：
    * 不同的type可以相互轉換/運算
    * 變數的structure完全一樣
*	Union type：
    *	將不同的datatype儲存在同一個記憶體空間的自訂型別
*	Primitive data types：沒有被其他資料類型定義的資料型態
*	Reference types : 可以間接存取記憶體的值的型別
*   Dangling pointers : 指向不合法記憶體位址的指標
*   Name type compatibility：兩個變數擁有相同的宣告或是使用相同的type宣告
*   Array : 相同型態的資料儲存在連續的記憶體
*	Fixed heap-dynamic array：
    * 固定的動態array，在需要使可以new出一個fixed的array
    * Storage binding is dynamic but fixed after allocation
*	Operator associativity rule | Operator precedence rule：
    * 定義同一優先級的operator之間關聯性的規則，如左關聯、右關聯
    * 運算子優先度一樣時，要決定如何運算，如從左到右、從右到左
    * Ex：A+B+C+D
         (((A+B)+C)+D) 左關聯
         (A+(B+(C+D))) 右關聯
*	Ambiguous grammar：相同的句子，可能造出兩種以上的parse tree
*   Smalltalk : A Pure OOP language
    *   Everything is objects
*   l-value：
    *   variable 的 address
    *   左值就是可以放在賦值操作符(等於=)兩邊的值
*   r-value:暫存值，不會在使用它的運算式之外保存
*   Functional side effect：調用函數時，還對主調用函數產生影響，例如修改全域變數
*   Inheritance：子類別從父類別獲得定義好的屬性和方法
*   Short-circuit evaluation :不用執行全部運算就能得出結果
    *   例:or運算，一個條件成立整個式子就成立
*   Ada : 
    *   美國國防部開發
    *   複雜難用
    *   幾乎將所有語言的特色都融入
*   Dynamic scope : 
    *   Based on calling sequences of program 
    *   從calling sequences of program才可以知道scope
*   Static scope : 
    *   Base on program text
    *   從program text就可以知道scope
### 非考古區
*    BNF : 用來描述language的language，一種meta language
*    multi-dimensioned array
     * rectangular : 只有一個指標，指到一塊連續記憶體
     * Jagged : 多個pointer指到1維陣列，形成多維
*    Assosiative array : 透過key去access (Hash...)
*    operation 動手做 很複雜
*    Axiomatic 根據邏輯做 也很複雜
*    denotation 根據數學 以funcuin實作
*    Explicit Declaration : 使用前要宣告型別
*    Implicit Declaration : 使用時會自動辨別型別
*    type inferencing : 例 2 (int) 與 2.0f(float)
*    Declaration order : 使用前就要宣告
     * int a; 這行之前都不能用a變數
*    reference counter : 參照計數，記憶體管理技術，是指將記憶體的被參照次數儲存起來，當被參照次數變為零時就將其釋放
*    stack dynamic : 從stack開始allocate，例 遞迴
*    exlicit heap dynamic : 從heap開始allocate，一般的動態配置記憶體
*    implicit heap dynamic : cause by assignment ，assign過程中產生的暫時動態配置記憶體
*    Referential transparency : 參照透明度，不更改程序行為的情況下將表達式替換為其相應的值
     * result1 = (fun(a)+b)/(fun(a)-c);
     * temp = fun(a);
     * result2 = (temp+b)/(temp-c);
     * if fun has no side effects -> result1 == result2 => Referential transparency
*    CIR (class instance record) : 存dynamic binding的資訊，EX : vtable(存虛函數的指標)
## BNF館 (第2大題)
*    **2019**
![](https://i.imgur.com/rcGSfr6.png)
*    **2017**
![](https://i.imgur.com/yjfxn7N.jpg)
*    **2013**
![](https://i.imgur.com/93DEBGu.jpg)
*    **2011**
![](https://i.imgur.com/mobV6X9.jpg)
*    **2007(答案是錯的)**
![](https://i.imgur.com/E7qIizI.png)
*    **2006**
![](https://i.imgur.com/0qcLWZb.png)

## BNF 二館 (第3、4大題)
*    **2019**
![](https://i.imgur.com/T5fIxT0.png)
![](https://i.imgur.com/EOAotIB.png)

*    **2017**
![](https://i.imgur.com/ut9X8kP.png)
![](https://i.imgur.com/gIaGMRc.png)

*    **2013**
![](https://i.imgur.com/ZtoDpKE.jpg)
![](https://i.imgur.com/FsB1Lz4.png)

*    **2012**
![](https://i.imgur.com/WLKdnpx.png)
![](https://i.imgur.com/fulN2ON.png)

*    **2011**
![](https://i.imgur.com/yKwqnD8.jpg)
![](https://i.imgur.com/qaQnjtA.jpg)

*    **2007**
![](https://i.imgur.com/wwXIW0U.png)

*    **2006**
![](https://i.imgur.com/oJJZ4to.png)

## Weakest precondition館 (第5大題)

*    **2019**
![](https://i.imgur.com/rDjpN5B.png)

*    **2017**
![](https://i.imgur.com/6flNtNa.png)

*    **2013**
![](https://i.imgur.com/aiUYRR6.png)
    
*    **2012**
![](https://i.imgur.com/GpOugKZ.png)

*    **2011**
![](https://i.imgur.com/iIr1rdx.jpg)

## Scoping館 (第6大題)
*    **2019**
![](https://i.imgur.com/4eorbgh.png)
*    **2017** 
![](https://i.imgur.com/XCNVg98.png)
*    **2013**
![](https://i.imgur.com/ypjh0PM.png)
*    **2012**
![](https://i.imgur.com/M2fTO9U.png)
*    **2011**
![](https://i.imgur.com/6nhMsmq.jpg)
*    **2007**
![](https://i.imgur.com/7m7baTO.png)
*    **2006**
![](https://i.imgur.com/ubJlAdZ.png)

