# <a name="up" />Проект Nation

Nation — сайт, который предоставляет информацию о различных турах, а также возможность бронирования и покупки мест на выбранные путешествия. Пользователи могут искать туры, узнавать о местах назначения, выбирать даты и оплачивать туры онлайн, обеспечивая удобство и доступность в путешествиях.

## Содержание
- [Задачи тестировщика](#задачи-тестировщика)
- [Требования по проекту](#требования-по-проекту)
- [Инструменты](#инструменты)
- [Проектирование тестовой документации](#проектирование-тестовой-документации)
- [Выполнение тестов](#выполнение-тестов)

## Задачи тестировщика

<details>
<summary> Задачи </summary> 

1. Изучить сайт [Nation](https://testlove.ru/test#form)
2. Спроектировать тест-кейсы для тестирования формы обратной связи
3. Выполнить тесты по тест-кейсу для тестирования формы обратной связи
4. Выполнить исследовательское тестирование, выявить дефекты и указать их (только заголовки)

***

</details>

## Инструменты
<p align="left"> 
  <a href="https://docs.google.com/" target="_blank" rel="noreferrer"><img src="https://w7.pngwing.com/pngs/240/1015/png-transparent-g-suite-google-docs-google-angle-rectangle-logo.png" width="36" height="36" alt="Google Sheets" /></a>
  <a href="https://www.jetbrains.com/youtrack/" target="_blank" rel="noreferrer"><img src="https://upload.wikimedia.org/wikipedia/commons/9/95/YouTrack_Icon.png" width="36" height="36" alt="Youtrack" /></a>
</p> 

## Объект тестирования
Сайт https://testlove.ru/test#form

## Проектирование тестовой документации
![Задание 2-3  Тест-кейсы, тестирование](https://github.com/SofiiaSleptsova/Nation/assets/147629405/f2aca430-a5f3-45c6-81f7-4b72d7ea41f0)
[Тестовая документация с кликабельными ссылками на баг-репорты](https://docs.google.com/spreadsheets/d/1asVxS0BCVHaFlcbOgEGqN0lc_Pd28gsPooxb24uO9-w/edit#gid=1368460235)

## Выполнение тестов
### Баг-репорты
<details>
<summary>ID: NATION-1 </summary>

### Данные отправляются с пробелом, если ввести их в начале и в конце значений в полях ввода в форме обратной связи (автоматический НЕ убираются) [NATION-1](https://slepsovasonya.youtrack.cloud/issue/NATION-1/Dannye-otpravlyayutsya-s-probelom-esli-vvesti-ih-v-nachale-i-v-konce-znachenij-v-polyah-vvoda-v-forme-obratnoj-svyazi)
 
**Предусловия:**  
1. Открыть сайт https://testlove.ru/test#  
2. Прокрутить до раздела "Забронировать тур"/нажать кнопку "Забронировать тур" в шапке  

**Шаги воспроизведения:**   
1. Заполнить поле "Ваша почта"/"Ваше имя"/"Выберите тур" c пробелом в начале или в конце  
2. Нажать на кнопку "Отправить"  

**Ожидаемый результат:**  
Данные отправляются без пробелов, если ввести их в начале и в конце значений в полях ввода в форме обратной связи (автоматический убираются)  
**Фактический результат:**     
Данные отправляются с пробелом, если ввести их в начале и в конце значений в полях ввода в форме обратной связи (автоматический НЕ убираются)  

**Приоритет:**   
Обычная  

**Окружение:**   
MacOS, Iphone 11  
Браузер: воспроизводится везде  

***
</details>

<details>
<summary>ID: NATION-3 </summary>

### В форме обратной связи, если поле ввода "Ваша почта" не заполнено, то данные отправляются [NATION-3](https://slepsovasonya.youtrack.cloud/issue/NATION-3)
 
**Предусловия:**  
1. Открыть сайт https://testlove.ru/test#  
2. Прокрутить до раздела "Забронировать тур"/нажать кнопку "Забронировать тур" в шапке  

**Шаги воспроизведения:**   
1. Заполнить валидными данными поле "Ваше имя"  
2. Заполнить валидными данными поле "Выберите тур"  
3. Нажать на кнопку "Отправить"  

**Ожидаемый результат:**  
В форме обратной связи, если поле ввода "Ваша почта" не заполнено, то данные НЕ отправляются, границы поля подсвечиваются красным и появляется текст об ошибке  
**Фактический результат:**     
В форме обратной связи, если поле ввода "Ваша почта" не заполнено, то данные отправляются  

**Приоритет:**   
Критическая   

**Окружение:**   
MacOS, Iphone 11  
Браузер: воспроизводится везде  

***
</details>

<details>
<summary>ID: NATION-4 </summary>

### В форме обратной связи, если в поле ввода "Ваша почта" ввести более 7 символов после точки в доменной части, то данные отправляются [NATION-4](https://slepsovasonya.youtrack.cloud/issue/NATION-4/V-forme-obratnoj-svyazi-esli-v-pole-vvoda-Vasha-pochta-vvesti-bolee-7-simvolov-posle-tochki-v-domennoj-chasti-to-dannye)
 
**Предусловия:**  
1. Открыть сайт https://testlove.ru/test#  
2. Прокрутить до раздела "Забронировать тур"/нажать кнопку "Забронировать тур" в шапке  

**Шаги воспроизведения:**   
1. Заполнить поле "Ваша почта" с более 7 символами после точки в домене  
2. Заполнить валидными данными поле "Ваше имя"  
3. Заполнить валидными данными поле "Выберите тур"  
4. Нажать на кнопку "Отправить"   

**Ожидаемый результат:**  
В форме обратной связи, если в поле ввода "Ваша почта" ввести более 7 символов после точки в доменной части, то данные НЕ отправляются, границы подсвечиваются красным и появляется сообщение об ошибке и данные не отправляются   
**Фактический результат:**     
В форме обратной связи, если в поле ввода "Ваша почта" ввести более 7 символов после точки в доменной части, то данные отправляются  

**Приоритет:**   
Критическая   

**Окружение:**   
MacOS, Iphone 11  
Браузер: воспроизводится везде  

***
</details>

<details>
<summary>ID: NATION-5 </summary>

### В форме обратной связи, если поле ввода "Ваше имя" не заполнено, то данные отправляются [NATION-5](https://slepsovasonya.youtrack.cloud/issue/NATION-5/V-forme-obratnoj-svyazi-esli-pole-vvoda-Vashe-imya-ne-zapolneno-to-dannye-otpravlyayutsya)
 
**Предусловия:**  
1. Открыть сайт https://testlove.ru/test#  
2. Прокрутить до раздела "Забронировать тур"/нажать кнопку "Забронировать тур" в шапке  

**Шаги воспроизведения:**   
1. Заполнить валидными данными поле "Ваша почта"  
2. Заполнить валидными данными поле "Выберите тур"  
3. Нажать на кнопку "Отправить"  

**Ожидаемый результат:**  
В форме обратной связи, если поле ввода "Ваше имя" не заполнено, то данные НЕ отправляются, границы поля подсвечиваются красным и появляется текст об ошибке   
**Фактический результат:**     
В форме обратной связи, если поле ввода "Ваше имя" не заполнено, то данные отправляются  

**Приоритет:**   
Критическая   

**Окружение:**   
MacOS, Iphone 11  
Браузер: воспроизводится везде  

***
</details>

<details>
<summary>ID: NATION-6 </summary>

### В форме обратной связи, если поле ввода "Выберите тур" не заполнено, то данные отправляются [NATION-6](https://slepsovasonya.youtrack.cloud/issue/NATION-6)
 
**Предусловия:**  
1. Открыть сайт https://testlove.ru/test#  
2. Прокрутить до раздела "Забронировать тур"/нажать кнопку "Забронировать тур" в шапке  

**Шаги воспроизведения:**   
1. Заполнить валидными данными поле "Ваша почта"  
2. Заполнить валидными данными поле "Ваше имя"  
3. Нажать на кнопку "Отправить"  

**Ожидаемый результат:**  
В форме обратной связи, если поле ввода "Выберите тур" не заполнено, то данные НЕ отправляются, границы поля подсвечиваются красным и появляется текст об ошибке  
**Фактический результат:**     
В форме обратной связи, если поле ввода "Выберите тур" не заполнено, то данные отправляются  

**Приоритет:**   
Критическая   

**Окружение:**   
MacOS, Iphone 11  
Браузер: воспроизводится везде  

***
</details>

## Баги сайта Nation
![Задание 1  Баги сайта](https://github.com/SofiiaSleptsova/Nation/assets/147629405/cd7e859d-3dfc-4ba4-828c-be751e6b39e2)
