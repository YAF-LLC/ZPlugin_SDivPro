# SDivPro

## 何ができるの?
スキャンデータなど、不必要に重たい or トポロジが汚いメッシュに対して、ディテールを保持したまま、サブディビジョンレベルを持っている、かつ、トポロジが綺麗なメッシュを生成するプラグインです。

具体的には、以下の一連の処理をワンクリックで行えるようになります。
1. 対象となるサブツールを複製
2. ローポリになるようにZRemesher適用
3. Divide, Project Allを必要な回数繰り返す

## 操作パネル (画像は英語ですが、日本語UIにも対応)
![Screenshot](/SDivPro_2021/doc/SDivPro.png)

### ZRemesher部分
ZRemesherの設定項目のうち、今回の目的で頻繁に調整する項目のみ抜き出してあります。

**Duplicate**のON/OFFスイッチは、ZRemesher適用前に複製を行うかどうかの設定に利用します。ZRemesherのパラメタを試行錯誤して調整する際には、手作業でメッシュを複製後、このスイッチをOFFにしてご利用ください。

ZScriptの仕様(？)のため、AdaptiveSizeとCurve Strengthのスライダーが実数値になっていますが、実際は整数に丸められた値が利用されます。

### Divide & Project All 部分
Divide(subdivide)とProject Allについての設定部分です。こちらも、頻繁に調整する項目のみ抜き出してあります。

**Max Subdiv Resolution** の項目で、必要なサブディビジョンレベルの最大を設定します(スクリーンショットの例だと、1～5のサブディビジョンレベルを持ったサブツールになります)。

### ワンクリックボタン
このボタンでは、上記のZRemesherとDivide&Project Allを一括で処理します(各パラメータはそれぞれのスライダーの値を利用します)。

## 導入方法
[Release](https://github.com/n-taka/ZBrush_SDivPro/releases/tag/v1.0)からSDivPro_2021.zipをダウンロード後、展開した中身をZBrushのプラグインフォルダに移動してご利用ください。

## 連絡先
[@kazutaka_nakash](https://twitter.com/kazutaka_nakash)

スライダーの初期値をカスタムしたいなどのご要望もウェルカムです。
