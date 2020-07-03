```
str: text
num> 42
txt|
	Lorem ipsum dolor sit amet
	on a single line!
arr>
	-> 42
	-: text
	-|
		multiline text
		goes here
	-
		this: here
		is: nesting
		woo>
			-: hoo
			-> true
```

```
str : text
num > 42
txt :>
	Lorem ipsum dolor sit amet
	on a single line!
arr >
	-> 42
	-: text
	-:>
		multiline text
		goes here
	->
		this : here
		is : nesting
		woo >
			-: hoo
			-> true
obj >
    foo : bar
    bar > 42
    qux :>
        Hello this is multiline.
        Yep it is.
```

```
str: text
num= 42
txt:
	Lorem ipsum dolor sit amet \
	on a single line!
arr>
	= 42
	: text
	:
		multiline text \
		goes here
	>
		this: here
		is: nesting
		woo>
			: hoo
			= true
	>	foo: bar
	>	>	deep: yeah
	>	>	nested= true
obj>
	foo: bar
	bar= 42
	qux:
		Hello this is multiline.
		Yep it is.
```
