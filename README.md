## android開発環境の構築


#### JDKのインストール
- [Java SE Development Kit 8 Downloads](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)からダウンロード。

#### Android Studioのインストール
- [1]の通りに実施。

#### Android SDKをインストール
- [1]の通りに実施。とりあえず、8.0,8.1,9.0をインストール

#### IntelliJ IDEAのインストール
- Android SDKを選択になかったので、Configure/PluginsでAndroid Supportにチェックを入れた（正直よくわからんが解決）。
- 設定の際にJDK,AndoroidのSDKの場所が分からなくてやや手間取った(結局,user/AppData/Local/Andorid/Sdkにあった)。
- いわれるがままにBuld Toolsをインストール。
- （ノートPCで）エミュレータがうまく動かなったのが、CPUの問題っぽいのであきらめた。

#### 実機でテスト
- [3]の通り実施で終了。

## 開発
- ストップウォッチの作成[2]。

## 参考サイト
[1] [IntelliJ IDEAでKotlin Androidアプリ開発環境構築！ 導入編](https://qiita.com/g0z4ru/items/24bca8e6fb691f29260f)  
[2] [正式採用の「Kotlin」で挑戦！ 初めてのAndroidアプリ開発 〜ストップウォッチを作ってみよう〜](https://employment.en-japan.com/engineerhub/entry/2017/06/23/110000)  
[3] [Android Studio】開発したアプリの実機テストを行う方法。](https://original-game.com/develop-android-app-4/)

