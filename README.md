# React-init-project

## 1  В пустой папке клонированного репозитория инициализировать React -
[`npx create-react-app my-app .`] 
    [`npm start`] - начало разработки / [`npm run build`] - билд проекта
    
## 2   В файл index.js автоматически при инициализации импортируеется:
    - `import React from 'react';`   не нужно импортировать в компоненты
    - `import ReactDOM from 'react-dom';`
    - `import './index.css';`
    
## 3   Установка зависимостей

   Установить в проект следующие пакеты.

    ```bash
    npm install --save-dev prettier husky lint-staged
    ```

   ## Интерграция плагинов .huskyrc и .lintstagedrc

   Добавить в корень проекта фалы .huskyrc и .lintstagedrc с кодом настроек внутри (скопировать)

  Ссылки на документацию по интеграции плагинов в популярные редакторы.
  - [Prettier editor integration](https://prettier.io/docs/en/editors.html)
  - [ESLint editor integration](https://eslint.org/docs/user-guide/integrations)

    ## Настройки VSCode

Для комфортной работы, после установки плагинов, нужно добавить несколько
настроек редактора в Settings VSCode для автосохранения и форматирования файлов.

    ```json
    {
      "files.autoSave": "onFocusChange",
      "editor.formatOnSave": true,
      "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
      }
    }
    ```
    
## 4   Нормализация стилей 1 из 2х вариантов

   - Встроенная нормализация
       `@import-normalize;`  в файл index.css  или App.css  
   - Внешняя нормализация   `npm install modern-normalize`  от  https://github.com/sindresorhus/modern-normalize
       `import 'modern-normalize/modern-normalize.css';`  в файл index.js

   
    
 
