# C-CPP-Snippets
C/C++ Snippets for faster coding, with explanation to apply in Atom

Snippets are basically autocomplete features offered by editors.
Some are present by default. You can modify existing snippets or add your own.

To use on Atom, go to Edit >> Snippets, which should open a snippets.cson file.
In the file, copy the code from the "snippets.cson" into it and save,
and you're ready to start using your snippets :)

Other Editors and IDEs will have something similar.

To add your own snippets or modify existing snippets do this

To add a snippet:
In the .cson file, first type '.source.cpp': , (use .c if you want exclusively for c).
 Then type the name/heading you want for your snippet 'while loop':
 Now in the next line type the 'prefix' (the key word seeing which the editor will suggest an autocomplete)
 type 'prefix': 'while'
 Now type the 'body' (what you want the editor to write), for example 'body': 'while (){\n}'
 This is will make the editor insert:
 
while (){

}

With your cursor after the final brace (there isn't an empty line between the braces)

If you had put 'body': 'while ($1){\n}'
 This is will make the editor insert:
 
while (){

}

With your cursor between the () of the while

Instead, if you had put 'body': 'while (${1:i}==42){\n}' the editor will insert:

while (i==42){

}

With 'i' being selected for you, and your cursor after i.
 You could also put multiple cursors simply by adding more "$1" signs.

You can experiment with other funcitonality too :)

To modify/overwrite a snippet:
You can copy the code for the existing snippet. In Atom you would go to Settings(Ctrl+,),
 open the language-c package, and scroll down to find the required snippet and click copy
(It's alright if you don't find the code).
 Now either copy the code and modify it, or write your own code the same way you did above.

You just need to remember to make sure the prefix you're using is the same as the one you want to modify,
 because if the prefix doesn't match, the original snippet will still behave the same way,
 and you would've only created a new snippet. If you've copied the code its fine, but otherwise
 make sure your prefix matches the prefix(key word) that the editor is using,

For example, there is snippet for struct which whose prefix is 'st' 
(this is the text you which the editor shows when start typing).
 So if you want to modify this, you need to use 'st' as your prefix 
to overwrite the previous snippet.

Hope you find my snippets useful! Modify you're snippets as per your need, and feel free to send suggestions.

PS: This will probably work for a different language as well :)
