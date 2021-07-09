# DB定義書
## ER図
[ERはこちら]

#DBテーブルカラム詳細一覧

###購入テーブル(d_purchase)
|和名| 属性名 | 型 | PK | NN | FX |
|:-------|----|---|---|---|
|オーダーID||bigint(20)|○|○||
||varchar(50)||○||
|purchase|deta||○||
|total_price|int(11)||○||

d_purchase_detail
| 属性名 | 型 | PK | NN | FX |
|-------|----|---|---|---|
|detail_id|bigint(20)|○|○||
|order_id|bigint(20)|○|○|○|
|item_code|int(11)||○||
|price|int(11)||○||
|num|int(11)||○||
