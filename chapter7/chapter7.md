# 第7章：商品と契約(前半)

## 商品と仕様特性

- 単純なモデル

![image](https://user-images.githubusercontent.com/44853475/139512018-792bb988-5d4e-4e4d-ab2b-a90a3c40ea4d.png)

	- ”焼肉溶岩プレート”だけを取り扱うユーザでない限り、サイズ、素材、標準売価だけは商品を管理できない
	- しかし、商品特性を思いつく限り属性として並べるわけにはいかない
		- キリがない
		- 仮にすべての商品特性を羅列できたとして、それが関係ない商品もある
			- 例えば”Tシャツ”なら「色」という属性に意味はある
			- しかし”米”だったら「色」という属性に意味はない


- 商品テーブル以外の場所に商品属性を保持するモデル

![image](https://user-images.githubusercontent.com/44853475/139512847-64d01626-d643-463a-b6fa-39fe5beb119e.png)

- インスタンスつき

![image](https://user-images.githubusercontent.com/44853475/139513144-69ededd0-7293-4036-b68d-5f33f7d545e8.png)

	- 管理属性Cと属性値がわかれば、商品Cを特定することができる

	- しかしこのやり方では、商品毎にどの属性を関連させるかはデータ管理者の判断にまかされる
		- 似た商品でも特定の属性が付与されたりされなかったり
		- 似たような管理属性がいくつも定義されたり

- 「品種」の考え方をとりいれたモデル

![image](https://user-images.githubusercontent.com/44853475/139513890-d7a46ea9-7952-4850-b8f9-020af65ddaf5.png)

再掲
![image](https://user-images.githubusercontent.com/44853475/139512847-64d01626-d643-463a-b6fa-39fe5beb119e.png)

![image](https://user-images.githubusercontent.com/44853475/139514303-4a3336d1-1cfd-4e83-b64d-1c67a9f090f2.png)

	- 「品種」毎に「属性の組み合わせ」をあらかじめ決めるモデル
	- 属性値の値はフリーに入力できる

## フィーチャ・オプション

- フィーチャ・オプション
	- フィーチャ　…　「顔」における”輪郭”や”目”といった要素(「顔の造作」「特徴」)
	- オプション　…　”タレ目””ツリ目”など、「目」のフィーチャがとり得る「オプション」
	- 略してFO

![image](https://user-images.githubusercontent.com/44853475/139514783-5afe8a9f-e735-4482-8ca2-8b01dfe85b02.png)

再掲
![image](https://user-images.githubusercontent.com/44853475/139513890-d7a46ea9-7952-4850-b8f9-020af65ddaf5.png)

![image](https://user-images.githubusercontent.com/44853475/139537713-12159b05-c8a8-41a8-9110-d7a496a4caf8.png)

	- 品種ごとの管理属性(フィーチャ)と、とり得る値(オプション)の両方をあらかじめ決めておけるようになった
	- しかし、この形式でもFOを「リスト形式」でしか定義できない
		- ”ケーブル長”といった数値系のフィーチャについては「範囲指定」したい
		- ”版”だったら、1.3.24といった固有の編集形式にしたい


## FO評価式の組み込み

![image](https://user-images.githubusercontent.com/44853475/139538543-fa398baf-333a-46f6-86b0-cee603485838.png)
![image](https://user-images.githubusercontent.com/44853475/139538564-c3b8b698-c382-4983-854b-b6b7ca6f26f3.png)

![image](https://user-images.githubusercontent.com/44853475/139538597-806fe504-295d-4aa8-854e-f3154a07aefb.png)

再掲
![image](https://user-images.githubusercontent.com/44853475/139514783-5afe8a9f-e735-4482-8ca2-8b01dfe85b02.png)

![image](https://user-images.githubusercontent.com/44853475/139538752-9f6abc3c-ffb2-48ff-93cd-aec7f4e91281.png)

## 製造品目

![image](https://user-images.githubusercontent.com/44853475/139561762-e303c1c3-0abe-4cc4-bacd-bba9e0f44be6.png)


## 部品表と工程表



