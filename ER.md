```startuml
@startuml
顧客マスタ}|..|| 購入テーブル
Entity03 }o..o| Entity04
Entity05 ||--o{ Entity06
Entity07 |o--|| Entity08
entity"顧客マスタ" as customer<m_customers>
<<M,MASTER_MARK_COLOR>>{
+customer_code[PK]
--

pass
name
address
tel
mail
del_flag
reg_date
}

entity"購入テーブル" as customer<d_purchase>
<<T,MASTER_MARK_COLOR>>{
+order_id[PK]
--
customer_code[FK]
purchase_date
total_price
}
entity"購入詳細テーブル" as customer<d_purchase_datan>
<<T,MASTER_MARK_COLOR>>{
+order_id[PK]
+detal_id[PK]
--
item_code[FK]
price
num

entity"商品マスタ" as customer<d_purchase_datan>
<<T,MASTER_MARK_COLOR>>{
+item_code[PK]
--
item_name
price
category_id[FK]
image
data

@enduml
```
