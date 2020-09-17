# react-dadata-suggestions-reactoutsideclick

## С чего начать

# Установка
`npm i --save react-dadata-suggestions-reactoutsideclick`

[страница на npm](https://www.npmjs.com/package/react-dadata-suggestions-reactoutsideclick)

# Описание

Библиотека форк "react-dadata-suggestions". Источник https://github.com/nobbynobbs/react-dadata-suggestions.
Выявлен баг.
Описание бага: Список закрывался при нажати на его скролл, что не давало проскролить список.
Для устранения бага была подключена библиотека "react-outside-click-handler" (https://github.com/airbnb/react-outside-click-handler), которая в сумме с небольшими изменения в коде библиотеки "react-dadata-suggestions" помогла устранить баг. Была произведена композиция компонента <DadataSuggestions /> в компонент <OutsideClickHandler /> и событие onBlur передано пропсом на родительский компонент (<OutsideClickHandler />), тем самым позволяя устранить вышеупомянутый баг.

