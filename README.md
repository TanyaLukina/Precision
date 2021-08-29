**Отчёт о тестировании приложения  Precision**

**Краткое описание**

25.07.2021 было проведено функциональное тестирование приложения  Precision.

На тестирование затрачено: 0,5 часа

В результате тестирования выявлены следующие дефекты: [Некорректный подсчет бонусов](https://github.com/TanyaLukina/Precision/issues/1#issue-952195354)

**Описание процесса тестирования**

В процессе тестирования использовались следующие артефакты:
[тест-кейс]( https://docs.google.com/spreadsheets/d/1NSOL0usZjwhTodzLEQnhTLZ5n_s3vQgpa7rnSEW8XBQ/edit?usp=sharing)



В качестве тестовых данных использовался следующий код.

```public class Main {
    public static void main(String[] args) {
        double regularBonus = 0.3;
        double specialBonus = 0.6;
        double totalBonus = regularBonus + specialBonus;
        System.out.println(totalBonus);
    }}
```

* Приложение запустилось и вернуло в консоли значение  "0.8999999999999999". Ожидалось значение "0.9".

**Тестирование производилось в следующем окружении:**

* Windows 10 Pro x64
* Java 11.0.11
* IntelliJ IDEA 2021.1.3 (Community Edition)
