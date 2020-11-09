## Отчет о тестировании программы Credit Card Number Validator

### Краткое описание

09.11.2020 был проведен Smoke Testing программы Credit Card Number Validator
Использовались следующие методы:
* граничные значения
* AD-Hoc

На тестирование потрачено: 1 час

В результате тестирования выявлены следующие дефекты:
* [Валидные карты не состоящие из 16 знаков не проходят валидацию](https://github.com/DariaPap/Java-Ex1.2/issues/1)

### Описание процесса тестирования

В процессе тестирования использовались следующие артефакты
* [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)
* [Сервис для генерации  валидных номеров карт](https://www.freeformatter.com/credit-card-number-generator-validator.html)

В качестве тестовых данных использовались
1. Номера карт сгенерированных на сервисе
* 4916938331923330 (VIZA)
* 4556805714292333044(VIZA)
* 6011643041713133 (Discover
* 6391292666527 (Diners Club International
* 6383507857234163 (InstaPayment)

2. Невалидные номера кредитных карт
* "creditcardnumber"
* "                " (16 пробелов)
*  "aaaaaaaaaaaaaaaa"
* "6"
* "12345678"

___________

Тестирование производилось в следующем окружении
* OS: Windows 10, 64 bit 
* Java Version OpenJDK 11
* IntelliJ IDEA 2020.2.3 (Community edition) Build #IC-202.7060.26