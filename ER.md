```startuml
@startuml
Entity01 }|..|| Entity02
Entity03 }o..o| Entity04
Entity05 ||--o{ Entity06
Entity07 |o--|| Entity08
@enduml
```
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
customer_code[FK]
purchase_date
total_price
}
