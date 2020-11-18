# 小テスト(仮)

## 1. Unix問題 全10点(各2点)

1. 今作業している場の一つ前に戻るには何と入力すれば最適か

2. 今いる場所にどのようなファイル、ディレクトリがあるかを確認するにはどうすれば良いか

3. 直前に使用したコマンドをもう一度使いたい時、何キーを押せば呼び出せるか

4. フォルダを作成したい場合、適切なコマンドはどれか
   - makedir
   - craftdir
   - cookdir
   - mkdir
5. ファイル等のリネームや移動を行うコマンドはどれか
   - remove
   - movie
   - rm
   - mv
## 2. Vi問題 全10点(各2点)

1. vim内でのカーソル移動に使うキーで適切なものはどれか
   - h,j,k,l
   - w,a,s,d
   - q,w,e,r
   - ←,↑,→,↓

2. 文字を挿入するのに使用するキーは何か

3. vim内のノーマルモードで[a]キーを押すと何ができるか

4. 行った作業を一つ前に戻すキーは何か

5. 文を一行削除したい場合に使用するコマンドはどれか
    - x
    - dk
    - dd
    - d$
## 3. Git問題 全10点(各1点)

1. .gitファイルをフォルダ内に作成するコマンドはどれか
   - git vivid
   - fit init
   - git commit
   - git init

2. gitの管理下にあるファイルの内容が変更された。確認をするために使用するコマンドは何か

3. 問2でファイルの変更を確認した。ステージングエリアに追加するコマンドは何か

4. 問3で無事追加出来たようだ。ではこの作業をコミットするのに使用するコマンドはどれか
   - git com
   - git commit
   - git combo
   - git graph

5. github内にあるリポジトリを初めてPCに取り込む場合、適切なコマンドはどれか
   - git pull
   - git push
   - git copy
   - git clone

6. local環境で編集したファイルをgithubに送信したい場合、適切なコマンドは何か
   
   - git push
   - git qush
   - git pull
   - git pool

7. branchを移動するコマンドは何か

8. 開発をするにあたって正しくない行動は以下の内どれか
   - 真面目に作業する
   - masterブランチで作業する
   - workブランチで作業する

9. 他の人の作業に加わるため自分のgithubに開発者のリポジトリを複製したい。適切な行動はどれか
   - Forkする
   - Porkする
   - Cokeする
   - あきらめる

10. PullRequestしたリポジトリの更新が活発で自分のリポジトリが遅れてしまっている。適切な行動はどれか
    - Fetch
    - Catch
    - Lunch
    - あきらめる
 
## 4. Html&css問題 全20点(各2点)

1. htmlを作成する時、&lt;!DOCTYPE　　　&gt;の空白の部分に入る文字は何か

1. htmlで使用する文字コードは何か

1. <p></p>は何か

1. 表を作る時に用いるコマンドは何か

1. htmlでコメントを残したい場合に使うコードは以下の内どれか

   - &lt;!-- --&gt;
   - //
   - /comment

6. cssで文字サイズを変更するプロパティは何か

1. cssで横幅を指定するプロパティは何か

1. 文字を中央に寄せるための宣言はどれか

   - font-align: center
   - text-align: center
   - font-align: inside
   - text-align: inside

9. padding: 10px 20px 30px;と指定されたとき、左側のpaddingはどれか？

   - 10px
   - 20px
   - 30px

10. 領域の角を丸めるプロパティは次のどれか？

    - border-lands
    - border-circle
    - order-rounded
    - border-radius

## 5. Java問題 全50点(各4点最後30点)

1. “java test”と表示するコードを作成してください(public class~等は不要)

1. System.out.printlnとSystem.out.printの違いは何か

1. 次の内正しいものはどれか

   - int x=エックス
   - int x=11
   - int x=X
   - int x=1.1

1. 数字等をランダムに出力したい場合に使うものはどれか

   - new Gundam().nextInt
   - new Random().nextInt
   - new Scanner().nextInt

1. %dや%sを使用して表示する場合の正しい選択を選んでください

   - System.out.println();
   - System.out.print();
   - System.out.printf();

1. 下のコードにはあからさまな間違いが10個ある。間違っている部分に取り消し線を引け(インデントのずれは無いものとする)

import japan.util.*;  
public class Ball{  
	public static voice main(String[] args){  
		int[] balls={1,2,3,4,5};  
		int[] isPicked={false,false,false,false,false};  
		for( i=0;i<5:i++){  
			while(true){  
				it index=new Pandom().nextInt(balls.length);  
				if(isPicked[index]){  
					continue;  
				}  
				System.out.prin(balls[index]);  
				isPicked[index]=true  
				breeak;  
			  }  
		}  
	}  
}
