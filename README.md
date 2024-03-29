# Тестовое задание для Junior Frontend разработчика

Разработать интерфейс для сайта [Hacker News](https://news.ycombinator.com/news), состоящий из двух страниц.

## Продуктовые требования
### Главная страница
- Показывает последние 100 новостей в виде списка, отсортированного по дате, самые свежие сверху.
- Каждая новость содержит:
	- название
	- рейтинг
 - ник автора
 - дату публикации
 - По клику на новость происходит переход на страницу новости
- Список новостей должен автоматически обновляться раз в минуту без участия пользователя
- На странице должна быть кнопка для принудительного обновления списка новостей
### Страница новости
- Должна содержать:	
  - ссылку на новость
  - заголовок новости
  - дату
  - автора
  - счётчик количества комментариев
  - список комментариев
- Корневые комментарии подгружаются сразу же при входе на страницу, вложенные - по клику на корневой.
- Список комментариев должен автоматически обновляться раз в минуту без участия пользователя
- На странице должна быть кнопка для принудительного обновления списка комментариев
- На странице должна быть кнопка для возврата к списку новостей

## Технические требования

- Приложение разработано с использованием React и Redux
- Использован [официальный API Hacker News](https://github.com/HackerNews/API). Вызовы Hacker News API и обработка данных от него производятся напрямую с фронтенда (кроме случая, если вы сделаете опциональное задание про Node.JS).
- Роутинг выполнен с использованием [React Router](https://github.com/ReactTraining/react-router/)
- Фреймворк UI любой (можно и без, на результат не влияет) на ваше усмотрение (как пример [React Bootstrap](https://react-bootstrap.github.io/) или [Semantic UI](https://react.semantic-ui.com/)).
- Пакетный менеджер `npm`
- Приложение должно запускаться по адресу `localhost:3000` командой `npm start`
- После запуска приложения все переходы по ссылкам не перезагружают страницу
- Исходный код решения должен быть выложен с вашего аккаунта на [Github](http://github.com/)

## Опциональные задания
- список комментариев в виде дерева
- Покрытие кода юнит-тестами
- Конфигурация сборки проекта в Docker image

