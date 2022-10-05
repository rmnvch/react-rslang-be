# RSLang. App for learning English. RS School JS / FE 2022 final project. Developed in team.
#### [App link](https://rslang-dpakyj1a.netlify.app/)
#### [Short video introduction link](https://youtu.be/nL61JKU79aI)
<h3>Overall description</h3>
This App is a single page application. It's based on collection of "Essential English Words" which includes 4000 words diveded into 6 categories according to difficulty levels. Words collection is stored using MongoDB and backend part is deployed on Heroku. We do not develop backend for this project as it was provided by school.
The App allows user to study english words through mini games - Sprint and Audio Challenge, add difficult words to vocabulary and to track learning process with statistics provided by the App.
<h4>App structure:</h4>
<ul>
<li>
  Main Page has links to games and welcome words.  
</li>
<li>
  Side Bar is available on the any page with the only exception of the game playing process. It has links to any part of page.  
</li>
<li>
  Textbook is the place where all words are being stored. It's divided into 6 categories 30 pages each category. Each category has its own color. There are links to games from textbook. If user launches game this way, only words from a current category will participate in game (excluding 'learned' words).
<br>User can mark words as 'learned' and as 'hard' (available only for authorized user):
<ul>
<li>'learned'. Once word marked as "learned" by user, App excludes this word from mini games if they are launched from textbook. In addition to that word can become 'learned' through learning process if there was given 3 right answers in a row in mini games</li>
<li>'hard'. The words labeled as 'hard' go to dictionary and participate in mini games launched from textbook. 3 right answers in a row makes word 'learned' and deletes this word from dictionary. Any mistake in a word makes it 'hard'</li>
</ul>
</li>
<li>
  Dictionary page is available only for authorized users. It stores 'hard' words. 
</li> 
 <li> 
   Games page has links to games. Available without authorization. Using this link to start the game user can choose difficulty level for game. All words will participate in game. 
  </li>
 <li> Team Page provides information about developers and their roles in the project. </li>
  </ul>
<h4>Additional UI features</h4>
<ul>
<li>
  User can enable or disable translation in word cards in Textbook.     
</li>
<li>
  Audio samples are available for each word in card and in results section after games.      
</li>
<li>
  Both games can be controlled by keyboard and mouse, fullscreen mode is available. User can disable sound for "sprint" game.      
</li>
</ul>

<h4>User technologies</h4>
TypeScript
<br>Webpack
<br>SCSS
<br>ESLint
<br>Prettier
<br>MongoDB
<br>Heroku for deploy
<br>Chart.js







# LearnWords
A backend part of [React RS.School task](https://github.com/rolling-scopes-school/tasks/blob/master/tasks/react/react-rslang.md)

#### [Wiki проекта](https://github.com/rolling-scopes-school/-LearnWords-react/wiki)  
#### [Swagger документация](https://react-learnwords-example.herokuapp.com/doc/#)
#### [Примеры запросов к API](https://github.com/rolling-scopes-school/-LearnWords-react/wiki/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B-%D0%B7%D0%B0%D0%BF%D1%80%D0%BE%D1%81%D0%BE%D0%B2-%D0%BA-API)

## Деплой

Сделайте форк репозитория и следуйте [инструкции по деплою и настройке приложения](https://github.com/rolling-scopes-school/-LearnWords-react/wiki).

## Локальный запуск
1. Создайте файл ```.env``` в корне приложения
2. В созданном файе укажите переменные окружения:  
```
PORT=<порт на котором будет запущено приложение>
MONGO_CONNECTION_STRING=<адрес вашей локальной или облачной mongodb>
JWT_SECRET_KEY=<ваш секретный ключ для подписи JWT>
JWT_REFRESH_SECRET_KEY=<ваш секретный ключ для подписи refresh JWT>
```
3. ```npm install```
4. ```npm run start:dev```
