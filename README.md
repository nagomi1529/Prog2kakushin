プログラム１について
テストの自分の点数と平均点を入力すると自分の点数の平均点と推移のグラフを出力するプログラム.
試験の自分の点数の推移を可視化することでモチベーションにつながる.
入力：input()関数から自分の点数と全体の平均点を入力.
出力：matplotlibのpyplotで推移のグラフを表示、pandasのDataFrameの集計処理で自分の点数の平均点を計算し出力.
工夫したところ：平均点との差を見れるようにしたところ.


プログラム２について
読み込んだ画像を90度回転させて保存するプログラム.
パソコンからだと横向きの方が見やすいけどスマホだと縦にした方が画像が大きく表示される.
入力：パソコンに保存した画像をGoogleドライブにダウンロードし、ColaboratoryからGoogleドライブにアクセスしてcv2.imread()で画像を読み込む.読み込んだ画像をkaiten()関数に代入する.
関数の内容：読み込んだ画像の各座標のRGBの数値を取得し、配列に格納.
　　　配列をnumpy.matrix()で行列に変換し、numpy.transpose()で転置した行列を取得.
      元の画像の幅と高さを入れ替えた大きさのグレー画像を新規作成.
      転置した行列に格納された画素の情報を、作成したグレー画像の各座標に代入.
      元の画像の幅と高さが逆になった画像ができる.
出力：元の画像を90度回転した画像を保存し、表示する.
画素の色の情報を行列にして転置することで座標の置き換えをシンプルにしたところ.


プログラム３について
読み込んだ画像の背景を取り除くプログラム.
シールやステッカーを作りたいときや、ほかの写真に合成したいとき背景を取り除いた部分を使用できる.
入力：globをインポートしておき、パソコンに保存した画像をGoogleドライブにダウンロードし、ColaboratoryからGoogleドライブにアクセスして、globで.pngがついているファイルを全て読み込む.
読み込んだ画像を順番にremoval()関数に代入する.
関数の内容：画像をImage.openで開いて、rembgモジュールのremove機能で背景の画像を取り除く.
　　　元の画像の名前に.pngを付けた名前で保存.
　　　背景が取り除かれた画像を表示.
出力：背景が取り除かれた画像.
工夫したところ：複数の画像をまとめて処理できるようにしたところ.
風景の写真などは上手く処理できないので入れてません.
rembgモジュールのremove機能を使用.
