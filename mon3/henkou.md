# 永続化方法の変更

## 1.概要
従業員マスタ、稼働マスタ、顧客マスタの３つのCSV形式のテキストファイルに保存して．  
いたデータをデータベースに保存するように変更する  

## 2.ユースケース図


## 3.イベントフロー


## 4.シーケンス図

### 4.1 「従業員情報を検索する」のシーケンス図

#### 4.1.1 「氏名から検索」のコードが選択された場合

#### 4.1.2 「職種から検索」のコードが選択された場合

## 5.クラス図

### 5.1. クラスの概要
|クラス名|概要|  
|:-------|:---|  
|SystemManager|従業員派遣管理メインクラス|  
|FileLoader|マスタファイルの読み込み処理を管理する|  
|NameSelectionStatus|検索する名前を入力する画面|  
|DisplayPersonByNameStatus|検索結果を一覧表示する画面|  
|DisplayPersonStatus|詳細情報を表示する画面|  
|TypeSelectionStatus|検索する職種を入力する画面|  
|DisplayPersonByTypeStatus|検索結果を一覧表示する画面|  

### 5.2. システムのクラス図

## 6.メソッド一覧

### 6.1 クラス SystemManager
|NO.|メソッド名|処理名|  
|:-:|:---------|:-----|  
|1|main|メインメソッド|  
|2|statusSetting|  

### 6.2 クラス ConsoleStatus
|NO.|メソッド名|処理名|  
|:-:|:---------|:-----|  

### 6.3 クラス NameSelectionStatus
|NO.|メソッド名|処理名|  
|:-:|:---------|:-----|  

### 6.4 クラス TypeSelectionStatus
|NO.|メソッド名|処理名|  
|:-:|:---------|:-----|  

### 6.5 クラス DisplayPersonByNameStatus
|NO.|メソッド名|処理名|  
|:-:|:---------|:-----|  

### 6.6 クラス DisplayPersonByTypeStatus
|NO.|メソッド名|処理名|  
|:-:|:---------|:-----|  

## 7. ファイル
検索からは従業員マスタ(person.csv)から検索
- 従業員マスタ(person.csv)
	- 従業員ID
	- 氏名
	- 住所
	- 電話番号
	- 職種
	- 勤続年数
	- 単価
	- 削除フラグ

## 8. システムの状態遷移図

## 9. 画面イメージ

### 9.1 最初の３件の表示画面

### 9.2 Nキーで次の３件
#### 9.2.1 次の３件を表示した画面

#### 9.2.2 次の３件がない場合に先頭から３件を表示した画面

### 9.3 Pキーで前の３件
#### 9.3.1 前の３件を表示した画面

#### 9.3.2 前の３件がない場合に末尾の３件を表示した画面