'''startuml
@startuml
Entity01 }|..|| Entity02
Entity03 }○..○| Entity04
Entity05 ||--○{ Entity06
Entity07 |○--|| Entity08
@enduml
'''
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
