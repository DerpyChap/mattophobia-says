# mattophobia-says
This is a Python library that is used for generating strings that what [Mattophobia](https://twitter.com/Mattophobia), COO of Nerd Cubed LTD, would say. This is a rewrite of the NPM package of the same name by Jack Baron, viewable here: https://unpkg.com/mattophobia-says@0.3.0/
## Example
```Python
#Import the library
from mattophobia-says import MattSays

#Setup the generator
generator = MattSays()

#Generate a random Matt string
print(generator.generate())
```
## Customization
`MattSays()` lets you submit your own lists of profanities to the generator if you feel like the current list of words aren't enough.
```Python
MattSays(swears, ings, standalone)
```

**swears** - A list of various swearwords 
**ings** - A list of words ending in "ing"
**standalone** - A list of standalone sentences that can be sent in place of a randomly generated string of swears.

You can customize the length of `MattSays().generate()` too:
```Python
MattSays().generate(min, max)
```
**min** - An int determining the minimum length of the string
**max** - An int determining the maximum length of the string

## Requirements

 - Python 3+ (Tested on 3.6, but should work on earlier versions)
