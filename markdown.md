# Markdown


## The Basics

### Line Breaks
To force a line break, put two spaces and a newlines (return) at the end of the line.

* This two-line bullet
won't break
* This two-line bullet  
  will break
  
Here is the code:

```
* This two line bullet
won't break

* This two line bullet  
will break
```
### Strong and Emphasize

**Strong**: `**Strong**` or `__Strong__`(Command-B)  
*Emphasize*: `*Emphasize*` or `_Emphasize_`[^emphasize]
 (Command-I)
 
### Header (like this one!)
	
	Header 1
	========
	
	Header 2
	--------
	
or

	# Header 1
	## Header 2
	### Header 3
	#### Header 4
	##### Header 5
	###### Header 6
	
	
### Links and Email
#### Inline
Just put angle brackets around an email and it becomes clickable:<qiuxunxun@yahoo.com>  
`<qiuxunxun@yahoo.com>`

Same thing with urls:<http://hsun.co>
`<http://hsun.co>`

Perhaps you want to some link text like this: [Hsun's blog](http://www.hsun.co "Title")  
`[Hsun's blog](http://www.hsun.co "Title")` (The title is optional)

#### Refence style
Sometimes it looks too messy to  you include big long urls inline, or you
want ot keep all you urls together.

Make [a link][arbitrary_id] `[a link][arbitrary_id]` then on it's own line 
anywhere else in the file:
`[arbitrary_id]: http://www.hsun.co`

If the link text itself would make a good id, you can link [like this][]
`[like this][]`, then on it's own line anywhere else in the file:
`[like this]: http://www.hsun.co`

[arbitrary_id]: http://www.hsun.co
[like this]: http://www.hsun.co

### Images
#### Inline
`![Alt Image text](path/or/url/to.jpg)`
#### Reference style
`![Alt Image Text][image-id]`  
or it's own line elsewhere:
`[image-id]: path/or/url/to.jpg "Optional Title"`
![google logo][]
[google logo]:https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png

### Lists

* Lists must be preceded by blank line (or block element)
* Unordered lists start each item with a `*`
- `-` works too
	* Indent a level to make a nested list
		1. Ordered lists are supported.
		2. Start each item (number-period-space) like `1. `
		42. It does't matter what number you use, I will render them sequentially
		1. So you might want to start each line with `1. ` and let me sort it out


Here is the code:
 
```
* Lists must be preceded by blank line (or block element)
* Unordered lists start each item with a `*`
- `-` works too
	* Indent a level to make a nested list
		1. Ordered lists are supported.
		2. Start each item (number-period-space) like `1. `
		42. It does't matter what number you use, I will render them sequentially
		1. So you might want to start each line with `1. ` and let me sort it out
```

### Block Quote
> Angle brackets `>` are used for block quotes.  
Technically not every line needs to start with a `>` as long as there are no empty lines between paragraphs.
> Looks kinda ugly though
> > Blcok quotes can be nested. 
> > > Multiple Levels
> 
> Most markdown syntaxes works inside
block quotes. 
> 
> * Lists
> * [Links][arbitrary_id]
> * Etc.


Here is the code

```
> Angle brackets `>` are used for block quotes.  
Technically not every line needs to start with a `>` as long as there are no empty lines between paragraphs.
> Looks kinda ugly though
> > Blcok quotes can be nested. 
> > > Multiple Levels
> 
> Most markdown syntaxes works inside
block quotes. 
> 
> * Lists
> * [Links][arbitraty_id]
> * Etc.

```

### Inline code
`Inline code` is indicated by surrounding it with backticks: `` `Inline code` ``

If your ``code has `backticks` `` that need to be displayed, you can use double backticks:``` ``Code with `backticks` `` ``` (mind the spaces preceding the final set of backticks)

### Block Code
If you indent at least four spaces or one tab, I'll display a code block.   

	print('This is a code block')
	print('The block must be preceded by a blank line')
	print('Then indent at least 4 spaces or 1 tab')
	print('Nesting does nothing. Your code is displayed Literally')

I also know how to do something called [Fenced Code Blocks](#fenced-code-block) which I will tell your later.

### Horizontal Rules
If you type three asterisks `***` or three dashes `---` on a line, I'll display a herizontal rule:

***

### Block Formatting
#### Table

This is a table:

First Header	|  Second Header  
-------------|---------------  
Content Cell	|	Content Cell  
Content Cell	|	Content Cell

| Left Aligned | Center Aligned | Right Aligned |
|:------- |:----------:|-------:|
|col 3 is   | some wordy text |$1600 |
|col 2 is   | centered  | $12 |  
| zebra stripes | are neat| $1|

The left- and right-most pipes(`|`) are only aesthetic, and can be omitted. The spaces don't matter, either. Alignment depends solely `:` marks.

### <a name="fence-code-block">Fenced Code Block</a>

This is a fenced code block:  

```
print("hello world!")
```

You can also use wave(`~`) instead of back ticks(`` ` ``):

~~~
print('hello world!')
~~~
