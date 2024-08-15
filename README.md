製品名		 : EZmachinelearning
作成者		 : HIapp
種別		 : machine learing app
開発環境	 : Python3.10.11
動作環境	 : Windows10にて動作確認
version		 : 1.0.1.0
更新内容	 : 

同梱ファイル 	 : ①EZmachinelearning
			|-- EZmachinelearning.exe
			|
			|-- assets
			|   |-- cartesian.png
			|   |-- custom_theme.json
			|   |-- settings.json
			|   |-- treeview_styles.json
			|
			|-- Tutorial_data
			|   |-- DataGeneration_demodata.csv
			|   |-- Decomposition_demodata.csv
			|   |-- OneHotEncoding_demodata.csv
			|   |-- Prediction_demodata_SSDSE-C-2023.csv
			|   |-- SMILESDescriptor_demodata.csv
			|   |-- Training_demodata_SSDSE-C-2024.csv

		　 ②readme

--------------------
◇使用方法◇
<Training>
①分析したいデータフレームのCSVファイルをインポート。
②CV値を設定(カンマ区切りで複数選択可)。
※データ数以上は選択できません。
※分類分析をする際は分類ターゲットのユニーク値以上にはできません。
③乱数を設定
④特徴量、ターゲット、分析モデルを選択
⑤学習開始
⑥学習が完了すると回帰分析結果の散布図、分類分析結果の混合行列、分析に使用したヒートマップ
モデル情報model.pklファイル、グリッドサーチの最適モデルパラメータ結果が保存されます。

<Prediction>
①分析したいデータフレームのCSVファイルをインポート。
②分析したいターゲット、モデルに対応するmodel.pklファイルを選択。
③出力するCSVファイルの文字コードを選択。
④予測開始
⑤予測が完了すると予測結果が保存されます。

<DataGeneration>
①データ生成用のデータフレームCSVファイルをインポート。
1行目 : step or array
stepの場合
2行目 : 系列名
3行目 : 最小値
4行目 : 最大値
5行目 : 刻み数
arrayの場合
2行目 : 系列名
3行目以降 : 任意
②生成チェックをし生成可能か確認。
③生成開始で生成

<OneHotEncoding>
①処理したいデータフレームのCSVファイルをインポート。
②処理する系列を選択。
③エンコーディングを実行。

<SMILESDescriptor>
①データ生成用のデータフレームCSVファイルをインポート。
1行目 : SMILES(固定)
2行目以降 : 任意の物質のSMILES
②生成する内容を選択
③出力開始で生成

<Decomposition>
①処理したいデータフレームのCSVファイルをインポート。
②処理する系列を選択。
③最終的な次元数と次元削減の方法を選択
※サンプル数以下にはできません。
④次元削減を実行。

<Setting>
言語と出力するフォルダを選択できます。


◇ 免責 ◇
・アプリ内の<Setting>をご参照ください
