# react-dadata-suggestions-reactoutsideclick

## С чего начать

# Установка
`npm i --save react-dadata-suggestions-reactoutsideclick`

[страница на npm](https://www.npmjs.com/package/react-dadata-suggestions-reactoutsideclick)

# Использование

Данная библиотека является копией(fork) библиотеки "react-dadata-suggestions". Источник оригинальной библиотеки https://github.com/react-dadata-suggestions.
В результате использования на проекте библиотеки "react-dadata-suggestions", были выявлен один баг. Описание бага: При вводе в инпут необходимого значения, нередко выводился список значений, если данный список имел множество значений появляся scroll, попытки пролистнуть список при нажатии ползунка скролла, приводили к закрытию списка (срабатывал onBlur). Для устранения бага была подключена библиотека "react-outside-click-handler" (https://github.com/airbnb/react-outside-click-handler), которая в сумме с небольшими изменения в коде библиотеки "react-dadata-suggestions" помогла устранить баг. Была произведена композиция компонента <DadataSuggestions /> в компонент <OutsideClickHandler /> и событие onBlur передано пропсом на родительский компонент (<OutsideClickHandler />), тем самым позволяя устранить вышеупомянутый бан

