**Unix(10)**  
・現在いる場所を確認するコマンドを書け  
pwd

・今のディレクトリにあるフォルダや隠しファイルを含めたファイルが表示されるコマンドを書け  
ls- la

・更新時間順にフォルダやファイルを並べてくれるコマンドを書け  
ls -lt

・一回でDesktopフォルダに移動するコマンドを書け  
cd ~/desktop

・一つ前にいた場所に戻るコマンド  
cd -

・ホームディレクトリに移動できるコマンドはどれか  
(1)cd home (2)cd .. (3)cd - (4)cd  
4

・vi file1.txtのコマンドを使用せずにfile1.txtにmemo1と書き込みを行うコマンド  
echo "memo1" &gt; file1.txt

・file1.txtファイルをコピーし同一フォルダ内にfile.2を作成するコマンドを書け  
cp file.txt file2.txt

・file2.txtをfileA.txtにリネームするコマンドを書け  
mv file2.txt fileA.txt

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
2yy

(2)bbbbbにカーソルがある状態で
その下に先ほどコピーした２行を5回貼り付けるコマンド
5p

(3)ページの最下段へ移動するコマンド
Sift G

(4)ページの最上段へ移動するコマンド
gg

(5)hljkそれぞれの移動方向を書け
h　左
l　右
j　下
k　上

(6)保存せずに終了する場合のコマンド
:q!


(7)コマンドiとコマンドA（Shift＋a)の違いを説明せよ
コマンドiはその場で挿入、Aは行末に挿入

(8)コマンドd$の機能を説明
カーソル位置から行末まで削除

(9)行頭へ移動するコマンド
0

(10)コマンドuで取り消しした作業を再び復元するコマンド
ctrl + r

**Git(10)**  
・作成したフォルダをgitの管理下に置くコマンド  
git init

・ファイル名であるtest.txtを指定してaddするコマンド  
git add test.txt

・最初のコミットと現在の作業フォルダの差分を確認するコマンド  
git diff

・devブランチを作成するコマンド  
git branch dev

・masterブランチからdevブランチに移動するコマンド  
git checkout dev

・masterブランチにdevの変更を取り込む手順  
（現在devブランチにいる場合)
git checkout master  
git merge dev

・リモートのgithubにpush&追跡設定をするコマンド  
git -u origin development  

**Html&css(20)**  
画像表現するタグはどれか？
(1)image(2)images(3)img(4)imege
3

CSSファイルを読み込むタグとして正しいのはどれか？  
(1)&lt;link rel="css" href="styles.css"&gt;  
(2)&lt;link rel="stylesheet" href="styles.css"&gt;  
(3)&lt;link rel="css" location="styles.css"&gt;  
(4)&lt;link rel="stylesheet" location="styles.css"&gt;  
2

箇条書きリストを作るタグの組み合わせとして正しいのはどれか？  
(1)li, ul  
(2)dl, li  
(3)li, ol  
(4)dl, dd  
1

空白の実体参照はどれか？  
(1)&amp;nbsp;  
(2)&nsbp;  
(3)&nbsp  
(4)&nsbp  
1

「行」「列」を表す英単語の組み合わせとして正しいものはどれか？  
(1)行 → width、列 → height  
(2)行 → height、列 → width  
(3)行 → column、列 → row  
(4)行 → row、列 → column  
4

CSSにおけるコメントの記述方法は次のどれか？  
(1)&lt;!-- comment --&gt;  
(2)/* comment */  
(3)// comment  
(4)// comment //  
2

CSSにおける長さの単位で正しくないのは次のどれか？  
(1)px  
(2)km  
(3)%  
(4)em  
2

黒を表すカラーコードを書け
#000000

白を表すカラーコードを書け
#FFFFFF

ボックスモデルに関する次の記述で正しいものはどれか？  
(1)marginの外側にborderがある。  
(2)marginとpaddingは同じ意味である。  
(3)paddingよりmarginの方が外側にある。  
(4)borderの外側にpaddingがある。  
3

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
3

5行目　*****の部分にあてはまるものを書け
items.length

7行目　int i = 3のときの出力結果を書け
何をしたはいくつ？

11行目で起きるエラーについて誤っている箇所と正解を書け
正：nextInt 誤：nextLine

16行目　(data[i].length)を(data.length)に書き換えた際に起こりうる不具合を書け  
入力される値に数字が依存するためエラーになる可能性がある

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
1~100

上記のif文を三項演算子で書き直せ  
ran > 50 ? "当たりです":"はずれです"

import java.util.*;を使用せずにランダムを出力するプログラムを書け
int ran = new java.util.Random().nextInt(100)+1;
