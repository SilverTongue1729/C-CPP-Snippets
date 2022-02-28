# C-CPP-Snippets
For Atom, go to `Edit >> Snippets`, which should open a `snippets.cson` file.
In the file, copy the code from the `snippets.cson` into it and save.

## To add a snippet:
- In the `.cson` file, first type `'.source.cpp':` , (use .c if you want exclusively for c).
- Then type the name/heading you want for your snippet `'while loop':`
- Now in the next line type `'prefix': 'while'` (the key word seeing which the editor will suggest an autocomplete)
- Now type the `'body'` (what you want the editor to write), for example `'body': 'while (){\n}'`
- This is will make the editor insert:
```cpp
while (){
}
```
- With your cursor after the final brace.
- If you had put `'body': 'while ($1){\n}'`, you're cursor will now be in between `()`
- Instead, if you had put `'body': 'while (${1:i}){\n$2}'` the you're cursor will intially be selecting `i`, and upon pressing tab the cursor will move to inbetween the braces in position of `$2`


For a multiline Snippet put the code between `'''<code>'''` instead of `'<code>'` in the body of the of the snippet

## To find for an existing snippet:
To copy the code for an existing snippet for C/C++ in Atom, you would go to `Settings`open the `language-c` package, and scroll down to find the required snippet, and copy the code.

## Modify a snippet
-  To modify an existing make sure the prefix you're using is the same as the one you want to modify. Else you would have created a new snippet and the old one will still remain
- For example, there is snippet for `struct` which whose prefix is `'st'`
- So if you want to overwrite this, you need to use 'st' as your prefix too.

## Disable a snippet
To disable a snippet type 'disabled': true

---

You could also check out Atom's default snippets from the language-c package,
or https://github.com/textmate/c.tmbundle

Hope you find my snippets useful!
