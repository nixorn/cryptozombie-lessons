---
title: Обзор урока
actions: ['Проверить', 'Подсказать']
skipCheckAnswer: true
material:
  saveZombie: false
  zombieResult:
    hideNameField: true
    ignoreZombieCache: true
    answer: 1
---

В Уроке 1 ты создашь «Фабрику Зомби» с целью собрать зомби-армию.

* Фабрика будет содержать данные всех зомби в армии
* У фабрики будет функция создания новых зомби
* У каждого зомби будет случайный уникальный внешний вид

В следующих уроках мы добавим больше функционала, например, сделаем так, чтобы зомби мог нападать на людей и других зомби! Но пока мы будем добираться до этого момента, напишем базовый функционал создания новых зомби.

## Как устроена ДНК зомби

Внешний вид зомби обусловлен его ДНК. ДНК зомби — простое целое число из 16 цифр, например:

```
8356281049284737
```

Как и в настоящей ДНК, различные части этого числа будут отражать специфические черты. Первые две цифры определяют внешний вид головы зомби, следующие две — разрез глаз и так далее.

> Примечание: это сильно упрощенный урок, поэтому у зомби возможно только 7 разных типов голов (хотя из 2 цифр можно получить 100 возможных вариантов). Если мы захотим увеличить число вариантов зомби, то потом добавим больше типов голов.

Например, первые 2 цифры зомби-ДНК, приведенной выше, равны `83`. Чтобы определить тип головы зомби, мы выполняем операцию `83 % 7 + 1` = 7. Этот зомби получит седьмой тип головы.

Чтобы увидеть, какой черте соответствует `83`, в правой панели сдвинь слайдер `head gene` (ген головы) до типа 7. Это шапка Санта Клауса!

# Попробуй!

1. Поиграй со слайдером в правой части страницы и увидишь, как различные цифровые комбинации соответствуют разным аспектам внешнего вида зомби.

Ладно, поигрались и хватит. Когда надоест, нажми на кнопку «Следующая глава» внизу страницы, и погрузись в изучение Solidity целиком!
