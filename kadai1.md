```uml
@startuml
start

:体力=10;

if(体力<=20)than(true)
:宿屋に泊まる;
else
:頑張ってレベルを上げる;
endif

end
@enduml
