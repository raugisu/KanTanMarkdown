# かんたんMarkdown
かんたんMarkdownは完全に単一のHTMLファイルで動作するMarkdownエディタ・プレビューアです。

次のURLにもう少し詳しい説明があります。

http://tatesuke.github.io/KanTanMarkdown/

## リリースノート

### v1.20160214.02

#### 機能追加・修正
* エディションを導入しました
 * ファイルサイズが最も小さいLiteエディション
 * 中くらいのStandardエディション
 * 最も大きいFullエディション

#### 内部改善
* jQuery依存排除により、Fullエディションでファイルサイズを約100Kb削減しました

### v1.20160214.01

#### バグ修正
* ctrl+s(cmd+s)で保存しても、保存されていないことになるバグを修正

#### 機能追加・修正
* エディタに変更があるとタイトルに「*」マークを付ける機能を追加
* 空のファイルは初期状態を編集モードにした

### v1.20160213.01

#### バグ修正
* キャレットが画面外に出てもスクロールバーが追従しないことがある問題を解決
* 特定の条件でキャレットが想定外の位置に飛んでしまう問題を解決

### v1.20160209.01

#### バグ修正
* Ctrl+Vを押しっぱなしにして連続ペーストした時にUndoが効かなくなる問題を解決

#### 機能追加・修正
* 初期状態では添付ファイル領域を表示させないようにした
* ファイルをドロップした時に添付ファイル領域を開くようにした

### v1.20160208.01

#### 仕様変更
* 「添付ファイルを隠す・表示する」、「プレビューを隠す・表示する」のショートカットキーをAltに変更  
Ctrl+→などは普通カーソル移動に割り当てられているため

### v1.20160207.01

#### バグ修正
* 再編集時1単語目でUndoするとカーソルが1文字目に戻ってしまう問題を修正(#66)


### v1.20160206.01

#### バグ修正
* コード中の<html>など特定のタグ文字列が保存時に消えてしまう問題を修正

#### 機能追加
* SafariやIE9など、保存ができない端末向けに「閲覧専用モード」を設けた
* オートインデントを導入
* 行選択でのインデント、アウトデントを導入
* MacOS向けのショートカットキーを追加

#### 内部修正
* テキストエリア周りのコードを改善

### v1.20160205.01

#### バグ修正
* IE, Firefoxにおいてtabキーが効かなくなっていたのを修正

### v1.20160204.02

#### バグ修正
* undoの挙動が不安定だったのを修正。これに伴いオートインデント機能を停止した

### v1.20160204.01

#### バグ修正
* 文章が横幅を超えてしまった時横スクロールバーが出てしまっていたが、改行するようにした

####機能追加・改善
* 閲覧モード時にプレビューの表示・非表示を切り替えられるようにした。
* エディタにオートインデント機能を追加した


### v1.20160203.01

#### 機能追加・改善
* ESCキーでを編集・閲覧モード切り替えられるようにしました
* 添付ファイル領域を表示非表示できるようにしました

#### 内部改善
* 一部のコードを改善しました

### v1.20160202.01
#### バグ修正
* firefoxでスクロールバー固定が効いていなかったのを修正
* 添付ファイル操作後に画面を閉じるとき、警告が出ていなかったのを修正

#### 機能追加、改善

* noscriptを追加

### v1.20160201.02

####バグ修正
* Firefoxで保存できていなかった致命的なバグを修正
* 閲覧モード時に保存をするとプレビューが真っ白になってしまう問題を修正

### v1.20160201.01

#### バグ修正
* IEで動作しなくなっていたバグを修正
* 横幅の大きなシーケンス図、フローチャットを描画したときにスクロールバーが二重に出てしまう問題を解決
* Firefoxで編集モード時にスクロールバーが二重に出ている問題を解決

#### 改善
* 閲覧モード時のレイアウトを改善しました

### v1.20160130.01

####バグ修正
・初期起動時にシンタックスハイライトが効いていないバグを修正

### v1.20160129.02

#### 仕様変更
* ファイルサイズの肥大化を防ぐため、保存時previewerの中身を削除するようにした

### v1.20160129.01

#### バグ修正
* 保存するとエディタやプレビューのスクロールバーが動いてしまう問題を解決
* ファイル末尾に不要タグが溜まっていく不具合を修正

#### 機能追加
* 自動更新のon/off機能を追加した

### v1.20160128_03

#### バグ修正

* 印刷時レイアウトが激しく崩れる問題を修正

### v1.20160128_02

#### 改善
* 閲覧モード時に横幅が大きすぎたので改善 

### v1.20160128_01

#### 改善
* h1がなくなった時のタイトルを[無題]にした

#### 機能追加
* info, warn, alertクラスを使うことで、青、黃色、赤枠を使えるようにした
* sequenceクラス,flowクラスを使うことでjs-sequence-diagramsとflowchart.jsを利用できるようにした


### v1.20160127_03

#### バグ修正
* スクロールバーが最下部で固定されないバグを修正

### v1.20160127_02

#### 改善
* プレビュー領域が最下部にある時は、内容更新後も最下部に固定するようにした
 + テキストエリアとプレビューのスクロールバー同期は難しそうだだったのでその代替案として
* 添付ファイルを削除する前にプロンプトを表示するようにした
* ソースコードハイライトの自動言語判定をやめ、手動指定にした

### v1.20160127_01

#### バグ修正
* 画像名を変更すると画像を表示できなくなっていたのを修正
* 画像名変更時にid属性から値を引っ張ってきているのを修正
* hrが表示されない不具合を解決

#### 機能追加、改善
* シンタックスハイライト導入
* テーブルの罫線が2重になっていたのを修正

#### 内部改善
* 画像をscriptタグに埋め込むとき、画像名はname属性に埋め込むようにした
* js内でファイルドラッグ時のスタイル適応をハードコーディングしていたのをやめた

### v1.20160126_01
* 保存のたびに</body>の前の改行が増えていくバグを修正
* MITライセンスとしました
* タブキーでタブが入力されるようにした

### v1.20160125_01
* ファイルを開いた時点では閲覧モードになるようにした
* 初期モードは閲覧モードにした
* 複数ファイル添付時の名前がおかしい問題を解決
* IEでも保存できるようにした

### v1.20160124_01
* リリース