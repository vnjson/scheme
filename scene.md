## Scene structure

_`input`__
```text
scenes
├───start
│   ├───assets
│   │   ├───background.png
│   │   └───audio1.mp3
│   ├───characters.yaml
│   ├───chapter1.yaml
│   ├───entry.yaml
│   └───label2.yaml    
├───lab
```

__`output`__
```text

game
├───scenes
│   └───en-US
│       ├───start.json
│       └───lab.json
└───assets
    ├───background.png
    └───audio1.mp3 
   
```


## Scene scheme
>__scene.json__
```json
{
  "assets": [
    {"name": "bg1", "url": "/assets/background-1.png"},
    {"name": "mainTheme", "url": "/assets/mainTheme.mp3"}
  ],
  "characters": [
    {"id": "al", "name": "Alice"}
  ],
  "label": [
    "Hello world!",
    {"alert": "This is work!"},
    {"scene": "bg1", "audio": "mainTheme"},
    {
      "menu": {
        "?": "What do you want to do?",
         "chapter2.start" :"I want to talk to Alice",
         "-10label": "I do not want to do anything"
      }
    }
  ],
  "-10label": [
    {"alert": "Game Over!", "point": -10}
  ]
}

```
>__chapter2.json__
```json
{
  "assets": [],
  "characters": [],
  "start": [
    {"al": "Hi my name is Alice"},
    {"jump": "gameOverLabel"}
  ],
  "gameOverLabel": [
    {"print": "Game over"}
  ]
}
```
## The scene is assembled from chunks of YAML

>__`characters.yaml`__
```yaml
- name: al      #require
  text: Alice   #require
  age: 17       #user params
  color: azure  #user params

- name: j
  text: John
  age: 21
  color: red
```
>__`label.yml`__
```yaml
- Hello world!
- alert: This is work!
- scene: bg1, 
  audio: mainTheme
- menu: 
   ?: What do you want to do?
   chapte2.start: I want to talk to John
  -10label: I do not want to do anything


```
>__`-10label.yml`__
```yaml
- alert: Game Over!
  point: -10
```
