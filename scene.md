

###Структура сцены *.json
>./scenes/ru-RU/start.json

```json
{
    "chapter1": [
      {
        "pr": "Привет! Давненько не виделись",
        "left":"prof_norm"
      },
      {
        "al": "Да уж, давненько.",
        "scene": "room_hero",
        "sound": "song1"
      },
      {
        "pr": "Хорош болтать! Погнали в лабараторию"
      },
      {
        "al": "Профессор вы слишком торопитесь. Это еще ни кому не помогало.",
        "scene":"roof"
      },
      {
        "pr": "Алиса не тебе меня поучать!",
        "left":"baka",
        "jump": "start/chapter2"
      }
    ],
    "chapter2": [
      {
        "al": "И как это понимать? Разве мы не должны позаботиться об этих ошибках?",
        "center": "errors",
        "sound": "errors"
      },
      {
        "pr": "Ты так ничему и не научилась..",
        "right": "chapter2"

      }
  ],
  "assets": [
    {
      "name": "background", 
      "extname": ".png", 
      "size": "14kb", 
      "path": "/background.png"
    }
  ]
}


```