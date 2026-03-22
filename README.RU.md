# SCSS Function Line Spacing

Пакет для интеграции функции расчета межстрочного интервала.

Документация: [EN](README.md) | [RU](README.RU.md)

___

## Установка

Вы можете установить пакет автоматически с помощью NPM:

```
npm i @bu0nq/scss-function-line-spacing
```

## Использование

Чтобы использовать этот пакет, импортируйте его в свой проект:

```scss
@use "@bu0nq/scss-function-line-spacing" as *;

.demo {
    line-height: line-spacing(16px);
}
```

## Изменение пространства имен

Вы можете изменить пространство имен во время импорта функции и использовать функцию с другим пространством имен:

```scss
@use "@bu0nq/scss-function-line-spacing" as function;

.demo {
    line-height: function.line-spacing(16px);
}
```

## Изменение переменных

Вы можете переопределить значения по умолчанию для указанных переменных при импорте функции:

```scss
@use "@bu0nq/scss-function-line-spacing" as * with (
    $interval: 1.5,
);
```
