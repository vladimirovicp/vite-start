# vite

Создадим проект на Vite:

```bash
npm create vite@latest
```

* Vanilla
* JavaScript
* default


В package.json вы увидите следующие скрипты в разделе scripts:

```
"dev": "vite",
"build": "vite build",
"preview": "vite preview"
```

```
"dev": "vite --open",
...
```


## Импорт JSON
Vite по умолчанию поддерживает импорт JSON-файлов. Это означает, что можно импортировать JSON-файл так же, как и любой другой модуль:
```
import data from "./data.json";
console.log(data);
```

## CSS
Vite позволяет добавлять стили через JS. В базовом шаблоне при развёртывании Vite приводится пример того, как это делать. В файле index.js есть следующий код:
```
import "./style.css";
```

## Статические ресурсы

Vite позволяет импортировать статические файлы прямо в JS-код. Например:

```
import image from "./img.png";
```

## Плагины

* **vite-plugin-minify** - можно добавить минификацию в сборку
