# VSCode 下使用用户自定义代码片段的简单介绍

## 目录
* [是什么](#用户自定义代码片段是什么)
* [怎么用](#如何使用用户自定义代码片段)

## 用户自定义代码片段是什么
代码段是一个模板，可让您更轻松地输入重复的代码。在VSC中，代码段会与其他建议一起出现在IntelliSense（Ctrl + Space）中。键入一个片段前缀（触发文本），然后按Tab或回车插入一个片段。

翻译自VSC官网。


## 如何使用用户自定义代码片段
### 如何进入用户自定义代码片段文件
进入VSC界面后，使用快捷键 `Crtl`+`Shift`+`P` 进入命令面板（如果你实在不想记快捷键，页面左下角有个齿轮，点开，选“命令面板”）。输入“配置用户代码片段”或者`Configure User Snippets`，回车，输入`latex.json`，再回车即可。

### 如何自定义用户自定义代码片段
无论是自定义还是直接把我定义好的.json文件直接粘走，都建议看看下面这一段，看懂这个才知道我都自定义了些啥，应该怎么用。

在latex.json文件前面有这样一段介绍：
```
// Place your snippets for latex here. Each snippet is defined under a snippet name and has a prefix, body and 
// description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
// $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the 
// same ids are connected.
// Example:
// "Print to console": {
// 	"prefix": "log",
// 	"body": [
// 		"console.log('$1');",
// 		"$2"
// 	],
// 	"description": "Log output to console"
// }
```
prefix 是在 Intellisense 中选择代码片段时要使用的前缀 body 片段内容。请使用 '$1', '${1:defaultText}' 来定义光标位置，使用“$0”表示最终光标位置。请插入带有“${varName}”和“${varName:defaultText}”的变量值，例如 "这是文件: $TM_FILENAME"。
description 代码片段描述。


## REFERENCE
https://github.com/sabertazimi/LaTeX-snippets
