## Base plugins
__`jump`__
```yaml
- jump: volume.chapter
```
```json
{
	"jump": "volume.chapter"
}
```
__`print`__
```yaml
- Some text
- print: Some text
```
```json
[
	"Some text",
	{"print": "Some text"}
]
```
__`character`__
```yaml
- al: Some reply
- john: Random reply
```
```json
[
	{"al": "Some reply"},
	{"john": "Random reply"}
]
```
__`menu`__
```yaml
- menu:
   ?: Some quetion
   label1: Menu item 1
   label2: Menu item 2

```
```json
{
	"menu": {
		"?": "Some quetion",
		"label1": "Menu item 1",
		"label2": "Menu item 2"
	}
}
```
