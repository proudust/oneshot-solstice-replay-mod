# OneShot Solstice Replay MOD

![Solstice Replay](https://user-images.githubusercontent.com/20186429/63818916-2a0bf600-c97e-11e9-8924-ae7d2b378abb.jpg)

## 概要
この MOD は通常 1 度しかプレイできない Solstice ルートをリプレイ可能にします。  
リプレイ時は通常ルートのリプレイ同様、ニコの歩行グラフィック及び顔グラフィックはワールドマシーンのものになります。  
導入前にセーブデータのバックアップをおすすめします。また、Windows でのみ動作します。  


## セーブデータのバックアップ

Windows 版の場合、`%APPDATA%\Oneshot\` がセーブデータの保存場所になります。  
セーブデータを復元する際、 Steam クラウドによるセーブデータ共有が ON だと正しく復元されないため注意してください。  


## 導入方法

1. [releases](https://github.com/proudust/oneshot-solstice-replay-mod/releases) から最新の MOD をダウンロードします。
2. ダウンロードした ZIP 内の `OneShot` フォルダを OneShot のインストールディレクトリに上書きします。
3. 上記スクショのように選択肢が増えていれば成功です。


## 改変内容

- Solstice クリア後のタイトルで *...* を選択したときの選択肢に *Solstice* を追加
- Solstice が選ばれた場合、Yes が選ばれたときの処理に加え、`%APPDATA%\Oneshot\` に `replay_solstice` ファイルを作成
- New Game 時に `replay_solstice` ファイルがあればそれを削除し、`[0152: Beat the game once]` スイッチを ON に設定
