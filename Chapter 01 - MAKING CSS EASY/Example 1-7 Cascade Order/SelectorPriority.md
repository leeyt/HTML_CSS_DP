Cascade Order
=============

Principle behind cascade order is to favor more specific selectors over general ones.

Selector group priorities (high to low):

1. rules marked with !important
2. inline style embedded using style attribute
3. rules with one more more ID selectors
4. rules with one or more class, attribute, or pseudo selectors
5. rules with one or more element selectors
6. rules with only universal selectors

If competing rules tied, resolve through location group.

Location group priorities (high to low):

1. <style> in <head> of HTML document
2. stylesheet imported through @import statement within <style> element
3. stylesheet attached by <link> element
4. stylesheet imported through @import statement within stylesheet attached by <link> element
5. stylesheet attached by end user (!important moves user-defined rule to highest priority)
6. default stylesheet supplied by browser

If still tied, rule placed later wins.
