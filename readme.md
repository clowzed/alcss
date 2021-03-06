<div align = "center">
    <h1>✨ ALCSS ✨</h1>
    <h2>Aligner of a splitter in css files</h2>
    
</div>


<br>

[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
<br>

[![Downloads](https://static.pepy.tech/personalized-badge/alcss?period=total&units=none&left_color=blue&right_color=brightgreen&left_text=pypi%20downloads)](https://pepy.tech/project/alcss)
<br>

[![CodeFactor](https://www.codefactor.io/repository/github/clowzed/alcss/badge)](https://www.codefactor.io/repository/github/clowzed/alcss)
![Example](./example.png)


## Requrirements
Check that you have:
- `python 3.x`
- `pip` (optionally)

## Installation
This program can be installed from [`pypi`](https://pypi.org/project/alcss)
```bash
py -m pip install alcss
pip3 install alcss
```

## Arguments

| short | long        | description                            | default |
|-------|-------------|----------------------------------------|---------|
| `-l`  | `--lmargin` | Sets spaces before `:` character       | `2`     |
| `-r`  | `--rmargin` | Sets spaces after `:` character        | `2`     |
| `-i`  | `--indent`  | Sets indentation inside {} block       | `4`     |
| `-s`  | `--shout`   | Forces program to print info to stdout | `False` |
| `-h`  | `--help`    | Shows help                             |         |


## Options meaning

```css
div {
____border_____:_____1px solid black;
↑           ↑     ↑
indent  lmargin rmargin
}
```

## Tips
- Use after default formmater of VS code as default formatter removes spaces before `:` character


- To add auto aligning after save:

- Add Run on Save extension
- Press ctrl + P and search for Preferences: Open Workspace Settings (JSON)
- Add code below into the opened file and save
```json
{
    "emeraldwalk.runonsave": {
        "commands": [
            {
                "match": ".css",
                "cmd": "alcss ${file}"
            }
        ]
    }
}
```

## Roadmap
* [✨] - ~~Make it work simply~~
* [❌] - Fix for nested brackets
