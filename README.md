```
# Tabbed Serialization Language (TAS)
# ---
# Example

# Simple strings:
title: Hello World!

# No need for quotes or escapes:
content: # : = > {} [] ' "

# Multi-line strings:
content:
	This string is actually
	on a single line.

	To add newlines, you put blank lines.

# Booleans:
isYaml= false

# Numbers:
num= 1,238,984.92

# Primitive vs string:
bool= true
boolstr: true
num= 42
numstr: 42

# Objects:
obj>
	foo: bar
	num= 64
	nest>
		baz: qux
		inner= true

# Arrays:
arr>
	>
		with newline= true

	>	without newline= true

	>	>	>	deep= true

	>
		>
			also deep= true

# ----------
# Edge cases
# ----------

# Special tokens in keys are escaped:
\#\:\=\>: value

# Empty string as key:
\: value

# Space as key
\ : value

# Whitespace as key:
\n\t: value

# Empty object:
obj>}

# Empty array:
arr>]
```
