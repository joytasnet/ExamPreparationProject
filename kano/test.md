**Unix(10)**  
・現在いる場所を確認するコマンドを書け  

・今のディレクトリにあるフォルダや隠しファイルを含めたファイルが表示されるコマンドを書け  

・更新時間順にフォルダやファイルを並べてくれるコマンドを書け  

・一回でDesktopフォルダに移動するコマンドを書け  

・一つ前にいた場所に戻るコマンド  

・ホームディレクトリに移動できるコマンドはどれか  
(1)cd home (2)cd .. (3)cd - (4)cd  

・vi file1.txtのコマンドを使用せずにfile1.txtにmemo1と書き込みを行うコマンド  

・file1.txtファイルをコピーし同一フォルダ内にfile.2を作成するコマンドを書け  

・file2.txtをfileA.txtにリネームするコマンドを書け  

・file1.txtを削除するコマンドを書け  
rm file1.txt


**Vi(10)**  
(1)  
aaaaa  
bbbbb

aaaaaの文章にカーソルがある状態で、
aaaaa
bbbbb
の二行をコピーするコマンド

(2)bbbbbにカーソルがある状態で
その下に先ほどコピーした２行を5回貼り付けるコマンド

(3)ページの最下段へ移動するコマンド

(4)ページの最上段へ移動するコマンド

(5)hljkそれぞれの移動方向を書け
h
l
j
k

(6)保存せずに終了する場合のコマンド

(7)コマンドiとコマンドA（Shift＋a)の違いを説明せよ

(8)コマンドd$の機能を説明

(9)行頭へ移動するコマンド

(10)コマンドuで取り消しした作業を再び復元するコマンド

**Git(10)**  
・作成したフォルダをgitの管理下に置くコマンド  

・ファイル名であるtest.txtを指定してaddするコマンド  

・最初のコミットと現在の作業フォルダの差分を確認するコマンド  

・devブランチを作成するコマンド  

・masterブランチからdevブランチに移動するコマンド  

・masterブランチにdevの変更を取り込む手順  
（現在devブランチにいる場合)
git checkout " "  
git merge " "  

・リモートのgithubにpush&追跡設定をするコマンド  
git "" development  

**Html&css(20)**  
画像表現するタグはどれか？
(1)image(2)images(3)img(4)imege

CSSファイルを読み込むタグとして正しいのはどれか？  
(1)&lt;link rel="css" href="styles.css"&gt;  
(2)&lt;link rel="stylesheet" href="styles.css"&gt;  
(3)&lt;link rel="css" location="styles.css"&gt;  
(4)&lt;link rel="stylesheet" location="styles.css"&gt;  

箇条書きリストを作るタグの組み合わせとして正しいのはどれか？  
(1)li, ul  
(2)dl, li  
(3)li, ol  
(4)dl, dd  

空白の実体参照はどれか？  
(1)&amp;nbsp;  
(2)&nsbp;  
(3)&nbsp  
(4)&nsbp  

「行」「列」を表す英単語の組み合わせとして正しいものはどれか？  
(1)行 → width、列 → height  
(2)行 → height、列 → width  
(3)行 → column、列 → row  
(4)行 → row、列 → column  

CSSにおけるコメントの記述方法は次のどれか？  
(1)&lt;!-- comment --&gt;  
(2)/* comment */  
(3)// comment  
(4)// comment //  

CSSにおける長さの単位で正しくないのは次のどれか？  
(1)px  
(2)km  
(3)%  
(4)em  

黒を表すカラーコードを書け

白を表すカラーコードを書け

ボックスモデルに関する次の記述で正しいものはどれか？  
(1)marginの外側にborderがある。  
(2)marginとpaddingは同じ意味である。  
(3)paddingよりmarginの方が外側にある。  
(4)borderの外側にpaddingがある。  

**Java(50)**
```java
 1 import java.util.*;
 2 public class Q1{
 3  public static void main(String[] args){
 4    String[] items = {"いつ","誰が","どこで","何をした",};
 5    String[][] data = [*****][];
 6    for(int i = 0; i < data.length; i++){
 7      System.out.printf("%sはいくつ?>",items[i]);
 8      int count = new Scanner(System.in).nextInt();
 9      for(int j = 0; j < data[i].length; j++){
10        System.out.printf("%sをいれて>",items[i]);
11        data[i][j] = new Scanner(System.in).nextInt();
12      }
13    }
14    String[] seps = {"、","が、","で、","。",};
15    for(int i = 0; i < data.length; i++){
16    int index = new Random().nextInt(data[i].length);
17    System.out.print(data[i][index] + seps[i]);
18    }
19    System.out.println();
20 }
21}

```
4行目 "何をした",}の「,」がない場合にどうなるか  
1.コンパイルエラーになる　2.コンパイルは通るが処理が実行されない　3.プログラムの作動に影響はない

5行目　*****の部分にあてはまるものを書け

7行目　int i = 3のときの出力結果を書け

11行目で起きるエラーについて誤っている箇所と正解を書け

16行目　(data[i].length)を(data.length)に書き換えたらどうなるか  
1.エラーになる　2.どちらも出力結果は変わらない　3.実行はされるが出力結果が異なる

```java
import java.util.*;
＊＊中略＊＊
int ran = new Random().nextInt(100)+1; 
if(ran > 50){
 System.out.println("当たりです");
}else{
 System.out.println("はずれです");
}
```
ranで出力される乱数の範囲を答えよ  

上記のif文を三項演算子で書き直せ  

import java.util.*;を使用せずにランダムを出力するプログラムを書け  
