
## Discription

Scenes are written in yaml and converted
to json. And the finished json is given to the interpreter.

Each keyword is an event

__`input`__
```yaml
- hello world
- print: some reply
- alert:
      msg: some
      param:  message
```
__`output`__
```json
[
	"hello world",
	{"print": "some reply"},
	{
	  "alert": {
	  	"msg": "some",
	  	"param": "message"
	  }

	}
]
```
__`execute`__
```js
//if ctx==="sting"
vnjs.on('print', data=>{
	console.log(data)
});
vnjs.on('alert', data=>{
	console.log(arg.msg+arg.param)
});

````

## Where use it?

* Text Quests

* Messenger bot text quest

* Visual novel

* Dialog system in game



## Tools
[__`scenes-to-json`__](https://github.com/vnjson/scenes-to-json) - Yaml scenes to json
 	
[__`YAML JavaScript exec`__](http://nodeca.github.io/js-yaml/) - Online Yaml linter


## Community
* [__`vk.com/vnjson`__](https://vk.com/vnjson)