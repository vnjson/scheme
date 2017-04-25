

###Структура сцены *.json
>./scenes/ru-RU/start.json

```json
{
  "labels":{
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
  ]
  },
  "assets": {
      "images": [
        "/background.png",
        "/right_ladya.png",
        "/lusil.png",
        "/hero_room.png"
      ],
      "audio": [
          "/song1.mp3"
      ]
  },  
  "characters": [
    {
      "aliase": "pr",
      "name": "Профессор",
      "color": "green"
    },
    {
      "aliase": "al",
      "name": "Алиса",
      "color": "red"
    },
    {
      "aliase": "ll",
      "name": "Люсиль",
      "color": "grey"
    }
  ]
}


```