# 　　作成者
<P>河原電子ビジネス専門学校<P>

<P>ゲームクリエイター科1年　森浩希</P>

# 1.　作品概要

<P><font size='5'>・Girl Revenge Story</font></P>

<P>2D横画面のターン制コマンドバトルRPGゲームです。</P>

<P><font size='5'>・使用エンジン</font></P>

<P>学校内製エンジンを使用。</P>

<P><font size='5'>・使用ツール</font></P>

<P>・visual Studio 2022</P>

<P>・Adobe Photoshop 2022</P>

<P>・Aseprite</P>

<P><font size='5'>・開発環境</font></P>

<P>Windows11</P>

<P><font size='5'>・制作人数</font></P>

<P>一人</P>

<P><font size='5'>・開発期間</font></P>

<P>2022年9月～2023年2月　（約三か月間）


# 2.　タイトル

<P>タイトル画面は、偽のタイトルの(GirlHeroStory)と本物のタイトルである（GirlRevengeStory）を使って、タイトル画面でAボタンを押すことにより、本来のタイトル画面を描画するようにしました。</P>

<P>これにより、ゲーム内でストーリーを説明せずとも、ユーザーが推測できる仕組みにしました。</P>

<P>偽のタイトル</P>

![](Title/GirlHeroStory.jpeg)

<P>本来のタイトル</P>

![](Title/GirlRevengeStory.jpeg)

<video controls src="Title/Title.mp4"></video>

# 3.　画面説明

<P><font size='5'>・ステージ</font></P>

<P>・十字キー（左右）　:　キャラ移動</P>

<P>・十字キー（上）　　:　マップ移動、ステージ選択</P>

<P>・Ｂボタン　　　　　:　ジャンプ</P>

<P><font size='5'>・戦闘</font></P>

<P>・十字キー（左右）　:　カーソル移動</P>

<P>・Ａボタン　　　　　:　決定</P>

<P>・Ｂボタン　　　　　:　キャンセル</P>

# 4.  操作方法
　
<P><font size='5'>・画面説明</font></P>

<P>・①　:　キャラクターのステータス</P>

<P>・②　:　キャラクター</P>

<P>・③　:　マップ移動の扉</P>

![](Manual.jpg)

# 5.  イラスト

<P>ゲーム内の素材はドットを打つ(Aseprite)を使って自作しました。</P>

![](Material.png)


# 6.  キャラクターのアニメーション
　
<P>キャラクターのアニメーションは複数の画像を変数の値で管理して、切り替えながら表示しています。


<P>戦闘モーション</P>

![](Any-Animations/Any-Fight.gif)

<P>立ちモーション</P>

![](Any-Animations/Any-Stand.gif)

<P>歩行モーション</P>

![](Any-Animations/Any-Walk.gif)

# 7.  場面切り替え

<P>ゲームの場面切り替えは下記のクラスを使用して実装しています。</P>

<P>1.場面切り替えのアニメーションを再生するクラス（SCREENCHANGEクラス）</P>

<P>2.キャラクターが居る場所を管理したクラス（ANY_MOVEクラス）</P>

<P>3.場所に応じた背景を描画するクラス（BACKGROUNDクラス）</P>

<video controls src="ScreenChange/ScreenChange.mp4"></video>

<P>場面の切り替えは違和感がないようにアニメーションでゲーム画面が覆われた際に2番と3番のクラスが起動して背景の画像を変更します。</P>

# 8.  ステージ

<P>K2Engineの使用上、2Dでカメラを扱うことができないのでキャラクターを動かす代わりに背景を動かしています。</P>

<video controls src = "ScreenChange/StageMove.mp4"></video>

# 9.  戦闘

<P>戦闘システムはドラゴンクエストで使われているターン制コマンドバトルを採用しています。</P>

<video controls src="ScreenChange/Fight.mp4"></video>