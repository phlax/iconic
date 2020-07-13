## iconic

Needs `Docker` permissions

For example...

```
cp -a example/assets assets
make icons
ls dist
```

### SVG 1


![SVG 1](/example/assets/bg.svg?raw=true "SVG 1")

### + SVG 2

![SVG 2](/example/assets/fg.svg?raw=true "SVG 2")

### + CONFIG

```json
[
    {
	"size": 140,
	"name": "example.png",
	"assets": [
	    {
		"src": "bg.svg",
                "scale": ".53",
                "x": 7,
                "y": 17
	    },
	    {
		"src": "fg.svg",
                "scale": "1.2",
                "x": 100,
                "y": 100
	    }
	]
    }
]

```

### = PNG

![PNG](/example/dist/example.png?raw=true "PNG")
