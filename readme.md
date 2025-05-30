# Тестовое задание

Репозиторий содержит базовый код страницы, а также данные, с которыми нужно работать.\
Склонируйте репозиторий в свой gitHub. Создайте ветку `review`. Создайте `pull-request` и запушьте все изменения в ветку `review`. Пришлите ссылку на `pull-request`. Не забудьте открыть публичный доступ к своему репозиторию.

### Макет находится по [ссылке](https://www.figma.com/design/MNlLp1RfXtV8LHgokCdj0S/LP?node-id=877-21&t=K0tKHOSOD5jSyk8d-1) (нужно запросить доступ)

**Сейчас страница выглядит так**\
 ![Скрин](./src/img/ScreenCurrentPage.png)

## В задании вам нужно:

**1. Реализовать переключение табов:**

- по `Таб 1` должен показываться список ссылок
- по `Таб 2` должна отображаться карусель баннеров

**2. На основе данных из `linksData.js` при помощи подготовленного шаблона `komus-links-item-template` отрисовать ссылки в контентной части первого таба.**

**3. Баннер с промокодом.**\
В контенте второго таба уже размещён баннер с промокодом. Вам необходимо реализовать:

- "обычный" тултип `Скопировать` при наведении на промокод
- "успешный" тултип `Скопировано` при клике на промокод
- задержку "успешного" тултипа на 3 секунды после клика
- запрет отображения "обычного" тултипа при наведении на промокод, пока отображается "успешный" тултип
- копирование промокода в буфер обмена при клике на промокод
- сохранение флага `promo` со значением `1` в локальное хранилище браузера при клике на промокод

**4. Баннер "Цена недели"**\
Также в контенте второго таба размещен баннер "Цена недели" с таймером. Вам необходимо настроить на таймере отсчёт в обратном порядке от 00:00 понедельника до 23:59 воскресенья. Таймер должен быть зацикленным, то есть каждый понедельник отсчет начинается заново.\
То есть в 00:00 понедельника таймер должен показывать `06 дней, 23 часов, 59 минут`.\
Будет плюсом, если реализуете смену значений для дней, часов и минут. То есть _дней-дня-день_, _часов-часа-час_, _минут-минуты-минута_.

**5. Баннерная карусель**\
Сейчас 2 баннера находятся друг под другом. Вам необходимо поставить их в ряд и настроить пролистывание карусели с зацикливанием. Пролистывание должно происходить по нажатию на стрелки в обе стороны. Также необходимо добавить пагинацию.\
Будет плюсом, если реализуете автопролистывание с задержкой 3-5 секунд. При этом при наведении мыши на карусель автопролистывание должно останавливаться.

## Заключение

Работайте со страницей `page1`. Можете настроить проект так, как вам удобно, добавлять папки и файлы, менять и добавлять разметку, стили и, конечно же, скрипты.\
Если вы видите, что в исходнике отсутствует разметка и/или стили какого-то компонента, значит подразумевается, что их нужно написать вам. Например, тултип.\
Старайтесь писать код JS декларативно и следовать принципу DRY (Don't Repeat Yourself), чтобы ту или иную логику вы могли потом легко переиспользовать на любых других проектах.

## Важно

Вся реализация должна быть выполнена нативными HTML, CSS и JS. Не используйте библиотеки, фреймворки, пре- и постпроцессоры, сборщики.
