---
title: スマートフォンが入るロボットの作り方【smabo】
date: 2023-12-03T09:02:46.000Z
categories:
  - smabo
  - robotics
id: "6801883189063756288"
draft: false
---
お疲れ様です。秋波です。

今回ご紹介するスマホが入るロボット、通称smaboは名前の通り**スマートフォンが入るロボット**です。

![smabo](https://akinami3.github.io/manage-hatenablog/images/smabo_introduction/smabo.png)


今では、殆どの人が持っているスマートフォンですが、

スマホを組み合わせたロボットがあれば面白いんじゃないか

と思いsmaboの作成を思いつきました。

<br>

本記事では、

- smaboの概要
- smabo作成の関連記事
- smabo作成に必要な部品

について説明します。

<br>

<div style= "font-size: 20px; font-weight: bold; background-color: lightgrey" > 目次 </div>
- [smaboでできること](#smaboでできること)
- [smabo関連記事](#smabo関連記事)
  - [基礎編](#基礎編)
  - [応用編](#応用編)
  - [発展編](#発展編)
- [必要部品](#必要部品)
    - [最小構成](#最小構成)
    - [共通](#共通)
    - [腕関連パーツ](#腕関連パーツ)
    - [頭関連パーツ](#頭関連パーツ)
    - [移動ロボット用パーツ](#移動ロボット用パーツ)
    - [ロボットアーム用パーツ](#ロボットアーム用パーツ)
    - [二足歩行用パーツ](#二足歩行用パーツ)
- [最後に](#最後に)



# smaboでできること

smaboでは

- ナビゲーション (navigation)
- 動作計画 (motion planning)
- 画像処理 (image processing)
- 遠隔操作 (remote control)
- 深層学習 (deep learning)
- 二足歩行 (bipedal walking)

など様々なことができます。

[https://twitter.com/akinami_robo/status/1719365981439692969:embed]

今後、smabo作成に関する様々な記事を公開していく予定ですが、smabo作りを通して、**ロボットの仕組みや動かし方を楽しく学ぶきっかけ**にできればいいなと思っています。

# smabo関連記事

smaboでは、様々なことが出来るため、内容別で記事を分けて解説していきます。

## 基礎編
基礎編では、

- 3Dプリンタを使ったsmaboの作成方法
- ラズパイ環境のセットアップ
- ROS2を使ったスマホとラズパイの通信
- 簡単なアクチュエータを使ったsmaboの制御
  
等について解説していく予定です。
<br>
<br>
なお、基礎編に関しては下記の記事一覧に記載の順番通りに進めていただくことを前提とした構成にする予定です。

<fieldset style="border:2px solid ; border-radius: 15px; box-shadow: 3px 3px 3px"><legend><span style="font-size: 16px;; font-weight:bold;">
記事一覧
</span> </legend>
    <ul style=" padding-left: 20px;">
        <li> smaboのボディを作ってみよう</li>
        <li>（事前準備）ラズパイとros2をインストールしよう</li>
        <li>smaboをROS2で通信してみよう</li>
        <li>smaboに腕を取り付けて制御してみよう</li>
        <li>smaboにカメラと超音波センサを取り付けてみよう</li>
    </ul>
</fieldset>


## 応用編
応用編では、

- 画像認識
- 機械学習
- 音声認識
  
など、基礎編より少し踏み込んだ内容について扱う予定です。
<br>
<br>
なお、応用編は基礎編の内容が完了している方は、どの順番でお読みいただいても成り立つ構成にする予定です。

<fieldset style="border:2px solid ; border-radius: 15px; box-shadow: 3px 3px 3px"><legend><span style="font-size: 16px;; font-weight:bold;">
記事一覧
</span> </legend>
    <ul style=" padding-left: 20px;">
<li> 【後日作成予定】smaboで画像認識してみよう
<li> 【後日作成予定】smaboで機械学習してみよう
<li> 【後日作成予定】smaboで音声認識してみよう
<li> 【後日作成予定】smaboとマイコンをmicro-ROSで通信してみよう</li>
    </ul>
</fieldset>


## 発展編
発展編では、

- 移動ロボット
- ロボットアーム
- 二足歩行ロボット

など、応用編より更に踏み込んだ内容について扱う予定です。
<br>
<br>
なお、発展編も応用編と同様に、基礎編の内容が完了している方は、どの順番でお読みいただいても成り立つ構成にする予定です。

<fieldset style="border:2px solid ; border-radius: 15px; box-shadow: 3px 3px 3px"><legend><span style="font-size: 16px;; font-weight:bold;">
記事一覧
</span> </legend>
    <ul style=" padding-left: 20px;">
<li>（事前準備）ラズパイとノートpcをros2で通信してみよう
<li>【後日作成予定】smaboを移動ロボットにしてみよう
<li>【後日作成予定】smaboにロボットアームを取り付けてみよう
<li>【後日作成予定】smaboを二足歩行ロボットにしてみよう
    </ul>
</fieldset>
# 必要部品

smaboでは、様々なことが出来るので項目別で「必要な部品」をまとめてみました。

<div style="padding: 1em; background-color: #DFF2BF; border-left: 6px solid #4F8A10; margin: 1em 0; border-radius: 5px; box-shadow: 0 2px 3px rgba(0, 0, 0, 0.5);">
    <h5 style="font-size: 15px; font-weight: bold; margin: 0 0 5px 0;">tips</h5>
    <p style="margin: 0;">「互換品多数あり」の商品に関しては、もっと安い商品があるかもしれないので、品質とのバランスを考えて互換品の購入も検討してみてください</p>
</div>

<div style="padding: 1em; background-color: #DFF2BF; border-left: 6px solid #4F8A10; margin: 1em 0; border-radius: 5px; box-shadow: 0 2px 3px rgba(0, 0, 0, 0.5);">
    <h5 style="font-size: 15px; font-weight: bold; margin: 0 0 5px 0;">tips</h5>
    <p style="margin: 0;">ピンヘッダがある部品に関しては、初心者の方でも使いやすい「はんだ付け済」の商品のURLを記載しています。<br><br>
ただし、「はんだ付け済み」は値段が高いことが多いので自身ではんだ付けできる方は「はんだ付けされていない」部品を買った方がお得です</p>
</div>

## 最小構成
|部品名|商品URL|
|---|---|
| Raspberry Pi<br>(4GB以上推奨) |-|
|スマートフォン<br>**Iphone MAXのような大きなサイズのスマホや、折り畳み式のような分厚いスマホは入らない**ので注意してください<br>pixel7a（152.0mm×72.9mm×9.0mm) + カバー でぎりぎりちょうどくらいのサイズです<br>それより小さいサイズに関しては「3Dプリンタで作成するスマホを入れる部分(phone_box)」のサイズを調整すればよいので問題ありません。|-|
| モバイルバッテリー（サイズが大きいとsmaboに入らないので注意。URLのAnker PowerCore Fusion 5000がちょうどいいくらいのサイズになります）| [url](https://www.amazon.co.jp/dp/B01LATWL5G?tag=pipinn-22&linkCode=ogi&th=1) |

## 共通 
|部品名|商品URL|
|---|---|
| ブレッドボード（85mm×55mm）<br>（サイズが大きいとsmaboに入らないので注意） | [url](https://www.amazon.co.jp/Clienmero-%E3%83%96%E3%83%AC%E3%83%83%E3%83%89%E3%83%9C%E3%83%BC%E3%83%89-%E3%82%B8%E3%83%A3%E3%83%B3%E3%83%91%E3%83%BC%E3%83%AF%E3%82%A4%E3%83%A4%E3%83%BC%E3%82%BB%E3%83%83%E3%83%88-%E9%9B%BB%E5%AD%90%E5%B7%A5%E4%BD%9C-%E5%8F%8E%E7%B4%8D%E3%82%B1%E3%83%BC%E3%82%B9%E4%BB%98/dp/B0BHZJLTL2?ref_=Oct_d_otopr_d_3332721051_6&pd_rd_w=X6yqu&content-id=amzn1.sym.41216987-bd79-42ee-9bcf-27052a070cb1&pf_rd_p=41216987-bd79-42ee-9bcf-27052a070cb1&pf_rd_r=D57C194X1NH6BZACFEPS&pd_rd_wg=FydDx&pd_rd_r=327745d6-16b1-418c-b484-4cea112fb00b&pd_rd_i=B0BHZJLTL2&th=1) |
| ジャンプワイヤー | [url](https://www.amazon.co.jp/ELEGOO-120pcs%E5%A4%9A%E8%89%B2%E3%83%87%E3%83%A5%E3%83%9D%E3%83%B3%E3%83%AF%E3%82%A4%E3%83%A4%E3%83%BC%E3%80%81arduino%E7%94%A8%E3%83%AF%E3%82%A4%E3%83%A4%E2%80%94%E3%82%B2%E2%80%94%E3%82%B828AWG-%E3%82%AA%E3%82%B9-%E3%83%A1%E3%82%B9-%E3%82%AA%E3%82%B9-%E3%82%AA%E3%82%B9-%E2%80%93%E3%83%A1%E3%82%B9-%E3%83%96%E3%83%AC%E3%83%83%E3%83%89%E3%83%9C%E3%83%BC%E3%83%89%E3%82%B8%E3%83%A3%E3%83%B3%E3%83%91%E3%83%BC%E3%83%AF%E3%82%A4%E3%83%A4%E3%83%BC/dp/B06Y48V9DL?ref_=Oct_d_obs_d_3332721051_0&pd_rd_w=uPj7Z&content-id=amzn1.sym.017d4a3b-167e-4891-9b01-9ac16ba095fb&pf_rd_p=017d4a3b-167e-4891-9b01-9ac16ba095fb&pf_rd_r=D57C194X1NH6BZACFEPS&pd_rd_wg=FydDx&pd_rd_r=327745d6-16b1-418c-b484-4cea112fb00b&pd_rd_i=B06Y48V9DL) |
| 単三×4 バッテリーボックス | [url](https://www.amazon.co.jp/%E3%82%AA%E3%83%BC%E3%83%A0%E9%9B%BB%E6%A9%9F%E5%B7%A5%E4%BD%9C%E3%83%BB%E3%83%9B%E3%83%93%E3%83%BC%E7%94%A8-%E5%8D%983%C3%974%E5%80%8B%E7%94%A8-%E3%82%B9%E3%82%A4%E3%83%83%E3%83%81%E3%83%BB%E3%82%AB%E3%83%90%E3%83%BC%E4%BB%98-%E3%82%B9%E3%82%A4%E3%83%83%E3%83%81%E3%83%BB%E3%82%AB%E3%83%90%E3%83%BC%E4%BB%98%E3%81%8DKIT-UM34-SK/dp/B001TRVXKY/ref=sr_1_8?keywords=%E9%9B%BB%E6%B1%A0%E3%83%9C%E3%83%83%E3%82%AF%E3%82%B9+%E5%8D%98%E4%B8%89+4%E6%9C%AC&qid=1700364271&sr=8-8) |
| 充電式単三電池 × 4 | [url](https://www.amazon.co.jp/Amazon%E3%83%99%E3%83%BC%E3%82%B7%E3%83%83%E3%82%AF-AmazonBasics-HR-3UTG-AMZN-%E5%85%85%E9%9B%BB%E5%BC%8F%E3%83%8B%E3%83%83%E3%82%B1%E3%83%AB%E6%B0%B4%E7%B4%A0%E9%9B%BB%E6%B1%A0-%E6%9C%80%E5%B0%8F%E5%AE%B9%E9%87%8F1900mAh%E3%80%81%E7%B4%841000%E5%9B%9E%E4%BD%BF%E7%94%A8%E5%8F%AF%E8%83%BD/dp/B00CWNMV4G/ref=sr_1_5?qid=1700364346&refinements=p_n_feature_thirteen_browse-bin%3A2314244051&s=electronics&sr=1-5&th=1) |
| 電池充電器 | [url](https://www.amazon.co.jp/%E3%80%90Amazon-co-jp%E9%99%90%E5%AE%9A%E3%80%91%E3%83%91%E3%83%8A%E3%82%BD%E3%83%8B%E3%83%83%E3%82%AF-%E6%80%A5%E9%80%9F%E5%85%85%E9%9B%BB%E5%99%A8-%E5%8D%983%E5%BD%A2%E3%83%BB%E5%8D%984%E5%BD%A2-%E9%BB%92-BQ-CC73AM-K/dp/B07FQJJ58Z/ref=sr_1_5?keywords=%E9%9B%BB%E6%B1%A0+%E5%85%85%E9%9B%BB%E5%99%A8&qid=1700402201&sr=8-5) |
| M2ネジ | [url](https://www.amazon.co.jp/dp/B08P1MNV9Z?ref=nb_sb_ss_w_as-reorder_k0_1_4&amp=&crid=1XGJ2MK2AE42S&amp=&sprefix=m2%E3%83%8D%E3%82%B8) |
| M3ネジ | [url](https://www.amazon.co.jp/gp/aw/d/B093GQ8FMJ/?_encoding=UTF8&pd_rd_plhdr=t&aaxitk=258063456cb7c90fbee9fd272b0939ff&hsa_cr_id=6156628800903&qid=1700402247&sr=1-1-ac08f2b1-eb5b-4f1a-aa64-9e8f448c33ed&ref_=sbx_be_s_sparkle_lsi4d_asin_0_title&pd_rd_w=moB6O&content-id=amzn1.sym.ea91fbda-5568-44df-b5b0-99202f731686%3Aamzn1.sym.ea91fbda-5568-44df-b5b0-99202f731686&pf_rd_p=ea91fbda-5568-44df-b5b0-99202f731686&pf_rd_r=5V3S0VPWGWSC2D0TDF9T&pd_rd_wg=2TOQq&pd_rd_r=3099d23a-4061-4c9a-b6fa-365d59d2ea0d) |
| サーボモータドライバ PCA9685（互換品多数あり） | [url](https://www.amazon.co.jp/HiLetgo-PCA9685-16%E3%83%81%E3%83%A3%E3%83%B3%E3%83%8D%E3%83%AB-12-%E3%83%93%E3%83%83%E3%83%88-Arduino%E3%81%AB%E5%AF%BE%E5%BF%9C/dp/B01D1D0CX2/ref=asc_df_B01D1D0CX2/?tag=jpgo-22&linkCode=df0&hvadid=218134682078&hvpos=&hvnetw=g&hvrand=18016470498878566809&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1009487&hvtargid=pla-439629573722&psc=1&mcid=d238c727398c34ec915ad739f9f6f977) |

## 腕関連パーツ 
|部品名|商品URL|
|---|---|
| SG90 × 2（互換品多数あり） | [url](https://akizukidenshi.com/catalog/g/gM-08761/) |

## 頭関連パーツ 
|部品名|商品URL|
|---|---|
| SG90<br>（互換品多数あり） | [url](https://akizukidenshi.com/catalog/g/gM-08761/) |
| Raspberry Pi Camera V2（互換品多数あり） | [url](https://www.switch-science.com/products/8940) |
| 超音波センサ HY-SRF05（互換品多数あり） | [url](https://www.amazon.co.jp/%E3%82%A2%E3%83%BC%E3%83%86%E3%83%83%E3%82%AF-86848-%E8%B6%85%E9%9F%B3%E6%B3%A2%E8%B7%9D%E9%9B%A2%E3%82%BB%E3%83%B3%E3%82%B5%E3%83%BC/dp/B00VFZ0JPK) |
| M1.6ネジ（HY-SRF05用） | [url](https://item.rakuten.co.jp/neji-matsumotosangyo/td-00111/) |
| RPLiDAR A1M8 |[url]( https://www.amazon.co.jp/RPLiDAR-A1M8-%E3%83%AC%E3%83%BC%E3%82%B6%E3%83%BC-%E3%82%B9%E3%82%AD%E3%83%A3%E3%83%8A-%E3%82%AD%E3%83%83%E3%83%88/dp/B07J9HSWJ6) |
| 照度センサ GY-30 | [url](https://www.amazon.co.jp/WINGONEER-GY-30-BH1750FVI%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E5%85%89%E5%BC%B7%E5%BA%A6%E3%82%BB%E3%83%B3%E3%82%B5%E3%83%A2%E3%82%B8%E3%83%A5%E3%83%BC%E3%83%ABI2C%E3%83%A9%E3%82%BA%E3%83%99%E3%83%AA%E3%83%BC%E3%83%91%E3%82%A4Arduino/dp/B06XHKTL58/ref=pd_lpo_sccl_2/358-3330547-6430326?pd_rd_w=yq6Fz&content-id=amzn1.sym.d769922e-188a-40cc-a180-3315f856e8d6&pf_rd_p=d769922e-188a-40cc-a180-3315f856e8d6&pf_rd_r=HAPBEA9R8KPW1BFMWFXD&pd_rd_wg=dyrHJ&pd_rd_r=9cd67c94-cb26-480c-bc15-4981c7694e75&pd_rd_i=B06XHKTL58&psc=1) |


## 移動ロボット用パーツ 
|部品名|商品URL|
|---|---|
| DCモータ + タイヤ（互換品多数あり） | [url](https://www.amazon.co.jp/KKHMF-3-6V%E3%82%AE%E3%83%A4%E3%83%BC%E3%83%89%E3%83%A2%E3%83%BC%E3%82%BF%E3%83%BC-%E3%82%B9%E3%83%9E%E3%83%BC%E3%83%88%E3%82%AB%E3%83%BC-%E3%83%AD%E3%83%9C%E3%83%83%E3%83%88%E3%82%BF%E3%82%A4%E3%83%A4-Arduino%E3%81%A8%E4%BA%92%E6%8F%9B/dp/B0915NPRFY) |
| エンコーダ付きDCモータ | [url](https://www.switch-science.com/products/6374/)|
| どこでもキャスターS | [url](https://www.amazon.co.jp/YAHATA-%E3%81%A9%E3%81%93%E3%81%A7%E3%82%82%E3%82%AD%E3%83%A3%E3%82%B9%E3%82%BF%E3%83%BC-S%E3%83%96%E3%83%AB%E3%83%BC-S/dp/B0091GH8YU) |
| TB6612FNG搭載 デュアルモータードライバ | [url](https://www.switch-science.com/products/3586) |

## ロボットアーム用パーツ
|部品名|商品URL|
|---|---|
| (SG90 ※ 頭のSG90と共通)（互換品多数あり） | [url](https://akizukidenshi.com/catalog/g/gM-08761/) |
| SG5010 | [url](https://akizukidenshi.com/catalog/g/gM-08913/) |
| SG92R | [url](https://akizukidenshi.com/catalog/g/gM-08914/) |
| SG90 （グリッパー用）（互換品多数あり） | [url](https://akizukidenshi.com/catalog/g/gM-08761/) |

## 二足歩行用パーツ
|部品名|商品URL|
|---|---|
| SG90 × 2（互換品多数あり） | [url](https://akizukidenshi.com/catalog/g/gM-08761/) |
| MG92B × 2 | [url](https://akizukidenshi.com/catalog/g/gM-13228/) |

# 最後に
本記事ではsmaboの概要についてご紹介しました。
<br>
<br>
具体的なsmaboの作り方については、別記事にて随時、解説してく予定です。
<br>
<br>
記事を公開次第、本ページの「smabo関連記事」の章も随時更新していくので、定期的にこのページを覗きに来てくださると幸いです。
