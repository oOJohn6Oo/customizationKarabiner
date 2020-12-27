# customizationKarabiner
karabiner key map script on my MacOS. mouse key included.

## 😄Default profile
> Default QWERTY config

* Simple modifications

| From key | To key |
| :----: | :----: |
| left_command | left_option |
| left_option | left_shift |
| left_shift | left_command |


* Complex modifications
	* Change right_option+ijkl to arrow keys
	* Change Ctrl+BackSpace to Fn+BackSpace(Delete)
	* Change caps_lock to control+-.(switch IME)
	* Maps button 5 to left desktop switch, 4 to right desktop switch,mc with button 3(mouse key)


## 😝Dvorak 
> 现有的键盘布局始终打不快字，所以想试试这种布局

* Simple modifications

| From key | To key |
| :----: | :----: |
| left_command | left_option |
| left_option | left_shift |
| left_shift | left_command |


* Complex modifications
	* Change right_option+chtn to arrow keys
	* Change Ctrl+BackSpace to Fn+BackSpace(Delete)
	* Change caps_lock to control+-.(switch IME)
	* Maps button 5 to left desktop switch, 4 to right desktop switch,mc with button 3(mouse key)


## karabiner json config file format
``` json
{
		"global": {
			...
		},
		"profiles": [
			{
				"name": "xxx"
				"simple_modifications": [
                	{
                    	"from": {
                        	"key_code": "xx"
                    	},
                    	"to": {
                        	"key_code": "xxx"
                    	}
                	},
					..
				],
				"complex_modifications": {
					"rules": [
						{
							"description": "change xxx to xxxx",
							"manipulators": ...
						},
						...
					]
				}
			},
			...
		]
}
```

## Installation

* 1. open ~/.config/karabiner/karabiner.json
* 2. copy the rules you like to the corresponding location
* 3. save it