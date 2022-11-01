# Sublime Text 4 setting

This repo contains all my configuration files, snippets and keybindings. Just clone the repository and replace the `User` folder after installing ST4 and the the `package control`.

## Specific settings

There are some packages that use a PC specific path:

- `citer`: just update the `bib` path according to the specific PC

## Keybinding

The general approach for a complete `keybinding` is:

```json
{
	   "keys": ["control+alt+c"],
	   "command": "insert_snippet",
	   "args": {
	    	"name": "Packages/User/rmd.sublime-snippet"
	   },
	   "context": [{
	   		"key": "selector",
    		"operator": "equal",
    		"operand": "text.html.markdown.rmarkdown"
    	}]
}
```

## Snippet

The general approach for a `snippet`:

```html
<snippet>
	<content><![CDATA[
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>rchunk</tabTrigger>
	<!-- <tabTrigger>hello</tabTrigger> -->
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>
```