# VSCode 下使用用户自定义代码片段的简单介绍

## 目录
* [是什么](#为什么要使用用户自定义代码片段)
* [怎么用](#如何使用用户自定义代码片段)

## 用户自定义代码片段是什么



## 如何使用用户自定义代码片段

### 文件存储路径

Crtl+Shift+P

### 使用方法介绍
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
prefix 在 Intellisense 中选择代码片段时要使用的前缀
body 片段内容。请使用 '$1', '${1:defaultText}' 来定义光标位置，使用“$0”表示最终光标位置。请插入带有“${varName}”和“${varName:defaultText}”的变量值，例如 "这是文件: $TM_FILENAME"。
description 代码片段描述。