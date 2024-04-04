# dataAnalyticsBasic データアナリティクスの基礎

[TOC]

## データサイエンスの基本
### データの構造化とデータマネジメント

#### データアナリティクスと問題解決
##### データアナリティクス
- データサイエンスに必要なスキル
    - データサイエンス(PC・AI・統計学)
    - データエンジニアリング力(意味ある形に実装・運用)
    - ビジネス力(課題を整理し解決)
##### 分析の目的
- 問題解決のための手がガリ
- 客観的な事実に基づいた科学的な意思決定
##### 情報倫理
- 機密処理
- 不正利用

#### 構造化データと非構造化データ
##### 量的変数と質的変数
- 量的変数: 数値的な量
- 質的変数: 分類を表す形
##### 構造化データと非構造化データ
- 構造化データ: テーブルデータ
- 非構造化データ: テキストデータや画像データ
##### ロングフォーマットとワイドフォーマット
- ロングフォーマット: 縦長のデータ
- ワイドフォーマット: 横長のデータ
##### 欠損値の対処
- リストワイズ(ケースワイズ)除去: 欠損値を含む行(列)を削除
- 代入法: 平均値や中央値などで代入する
    - 多重代入法
    - 期待値代入法
##### 層別パレート分析

## 質的データのアナリティクス
### 重点志向とパレート分析
#### パレート分析の手順とパレート表
##### パレート表
- 頻度とコストで評価
##### パレート図
- コストを棒グラフで、頻度を折れ線グラフで表したもの
#### 層別パレート分析
- クロス集計表の作成
- 特化係数
    - 特化係数が1であれば、部分集団の割合が全体集団と同じ
    - 1より離れた値をとると、交互作用効果があることを意味する 
$$ 特化係数 = \frac{部分集団の割合}{全体集団の割合} $$

### データ項目間の関連性とクロス集計分析
#### クロス集計表
##### 周辺分布に関する問題
- 「商品への関心」に関する周辺分布
- 「スポーツ中継」に関する周辺分布

| sports\interest | ある  | ない  | 周辺分布 |
| :-------------: | :---: | :---: | :------: |
|     みない      |  131  |  53   |   184    |
|      みる       |  68   |  188  |   256    |
|    周辺分布     |  199  |  241  |   440    |

##### 同時分布に関する問題

- 二つの質的データの同時分布

| sports\interest | ある  | ない  |
| :-------------: | :---: | :---: |
|     みない      |  131  |  53   |
|      みる       |  68   |  188  |

- 総計に対する割合

| sports\interest | ある  | ない  | 周辺分布 |
| :-------------: | :---: | :---: | :------: |
|     みない      | 29.8% | 12.0% |  41.8%   |
|      みる       | 15.5% | 42.7% |  58.2%   |
|    周辺分布     | 45.2% | 54.8% |  100.0%  |

##### 条件付分布に関する問題

- 商品の関心の条件付分布

| sports\interest | ある  | ない  | 周辺分布 |
| :-------------: | :---: | :---: | :------: |
|      みる       | 26.6% | 73.4% |  100.0%  |
|     みない      | 71.2% | 28.8% |  100.0%  |
|      Total      | 45.2% | 54.8% |  100.0%  |

- スポーツ中継の条件付分布

| sports\interest |  ある  |  ない  | 周辺分布 |
| :-------------: | :----: | :----: | :------: |
|      みる       | 34.2%  | 78.0%  |  58.2%   |
|     みない      | 65.8%  | 22.0%  |  41.8%   |
|      Total      | 100.0% | 100.0% |  100.0%  |

- 条件付(構成)割合に明らかな違いが**ある**とき、二つの質的変数の間には**関連がある**
- 条件付(構成)割合に明らかな違いが**ない**とき、二つの質的変数の間には**関連がない**

#### 連関係数と $\chi^2$ 検定 ~関連性の強さを見る~

##### 観測度数と期待度数



##### 二つの変数に関連がないことを仮定したときの期待度数



##### $\chi^2$ 統計量: 観測度数の期待度数からの乖離



##### クラメールとピアソンの連関係数


##### $\chi^2$ 検定: 母集団における関連性の検定


##### 

## 量的データのアナリティクス
### 分布構造の把握と基本統計量
### 相関・予測と回帰分析

## 確率・確率分布・推測のアナリティクス
### 確率に基づく判断
### 統計的な推測

## 時系列・テキスト・乱数データのアナリティクス
### 時系列データの分析
### テキストデータの分析
### シミュレーションと乱数

## 実践模擬問題
### 模擬問題と解答