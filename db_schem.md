<h1> データベースの詳細</h1>

d_purchase
| 属性名 | 型 | PK | NN | FX |
|-------|----|---|---|---|
|order_id|bigint(20)|○|○||
|customer_code|varchar(50)||○||
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
