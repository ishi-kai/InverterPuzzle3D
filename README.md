# InverterPuzzle

CMOSプロセスで設計したインバータ（NOTゲート）のレイアウトと3次元構造を模したアクリルパズルの加工データです。

## 用意するもの
- 3mmアクリル板（透明）
- 3mmアクリル板（黒）
- 薄い透明シート（OHPシート、トレーシングペーパー等）

## 作り方
- 3mmアクリル板を、inv_cut.pdf（一番下の横長長方形以外は透明板。右下の5mm角正方形部品は黒色板）でレーザーカッター等でカットします。（5mm角の正方形の部品（コンタクトホール）がなくなりやすいので注意）
- 薄い透明シートを、inv_cut.pdfの一番下の横長長方形の形状にカット（ゲート酸化膜）
- UVプリンタで、inv_UV_print.pdfのデータを、カットした部品を並べて印刷。このときinv_UV_base.pdfをアクリル板等でカットしておくと位置合わせがやりやすい。

## 組み立て方
以下のレイヤと色の対応をみながら、インバターのレイアウトをつくります。
- 薄ピンク: Psub
- 薄緑: Nwell
- ピンク: P+
- 緑: N+
- 透明: 酸化膜
- 赤: PolySi
- 水色: Metal1
- 黒: CNT（コンタクトホール）

## Author

Junichi Akita (akita@ifdl.jp / @akita11)


# InverterPuzzle3D

CMOSプロセスで設計したインバータ（NOTゲート）のレイアウトと3次元構造を模した3Dプリントパズルの加工データです。

## 用意するもの
- 3Dプリンター（積層型、光造形型どちらでもOKです）
   - 各レイヤーの色に合わせた3Dプリンター用フィラメント or レジン
- 4mm直径2mm厚の円形磁石
- 2mm直径1mm厚の円形磁石

## 作り方
- InverterPuzzle3D_[レイヤー名]_[色]_[部品番号].stlをそれぞれの[色]のフィラメントまたはレジンで印刷
- 各部品の4mm直径と2mm直径の穴に磁石をはめ込む

## 組み立て方
以下のレイヤと色の対応をみながら、インバターのレイアウトをつくります。
- クリアレッド: Psub
- クリアグリーン: Nwell
- 紫: P+
- 緑: N+
- 透明: 酸化膜
- オレンジ: PolySi
- 水色: Metal1
- クリアブルー: Metal2
- 黒: CNT（コンタクトホール）1レイヤー分 * 5個
- 黒: CNT（コンタクトホール）2レイヤー分 * 7個


### 各レイヤー例
- シリコン層その1：P Sub ![シリコン層その1：P Sub](/images/InverterPuzzle3D_P-Sub_ClearRed.jpg)
- シリコン層その2：N Well ![シリコン層その2：N Well](/images/InverterPuzzle3D_N-Well_ClearGreen.jpg)
- シリコン層その3：N+とP+ ![シリコン層その3：N+とP+](/images/InverterPuzzle3D_N-Plus_Yellow-P-Plus_Purple.jpg)
- 酸化膜層 ![酸化膜層](/images/InverterPuzzle3D_GateOxide_Clear.jpg)
- 第3層とシリコン層のコンタクト層 ![第3層とシリコン層のコンタクト層](/images/InverterPuzzle3D_CNT-VIA_Black_2layer-GateOxide_Clear.jpg)
- 第3層：ポリシリコン層 ![第3層：ポリシリコン層](/images/InverterPuzzle3D_POL_Orange.jpg)
- 第2層と第3層のVIA層 ![第2層と第3層のVIA層](/images/InverterPuzzle3D_POL_Orange-CNT-VIA_Black_1layer.jpg)
- 第2層：メタル層その1 ![第2層：メタル層その1](/images/InverterPuzzle3D_ML1_SkyBlue.jpg)
- 第1層と第2層のVIA層 ![第1層と第2層のVIA層](/images/InverterPuzzle3D_ML1_SkyBlue-CNT-VIA_Black_1layer.jpg)
- 第1層：メタル層その2 ![第1層：メタル層その2](/images/InverterPuzzle3D_ML2_ClearBlue.jpg)


## Author

Noritsuna Imamura (noritsuna@ishi-kai.org / noritsuna@siprop.org / @noritsuna)
