# Контекст решения
<!-- Окружение системы (роли, участники, внешние системы) и связи системы с ним. Диаграмма контекста C4 и текстовое описание. 
-->
```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml

Person(user, "Пользователь")

System(conference_site, "Сайт магазина", "Веб-сайт магазина для продажи товаров")



Rel(user, conference_site, "Регистрация, просмотр/изменение информации о блогах и публикациях")



@enduml
```
## Назначение систем
|Система| Описание|
|-------|---------|
| Сайт магазина | Веб-интерфейс, обеспечивающий доступ к информации товарам, имеющимся в магазине. Бэкенд сервиса реализован в виде микросервисной архитектуры |

