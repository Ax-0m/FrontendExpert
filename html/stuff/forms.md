# Forms

The bread and butter of user input. Master these and you're good to go.

## Basic Structure

**Form** `<form>`  
Wrap everything in this. Your team comp container.

**Input** `<input>`  
Self-closing. Does the heavy lifting with different `type` attributes.

**Label** `<label>`  
Describes what each input does. Use `for` attribute to link with input's `id`.

## Common Input Types

**Text** `type="text"`  
Basic text input. Your safe pick.

**Email** `type="email"`  
Email validation built-in.

**Password** `type="password"`  
Hides the text as you type.

**Submit** `type="submit"`  
Button that sends the form data.

**Checkbox** `type="checkbox"`  
For yes/no or multiple selections.

**Radio** `type="radio"`  
One choice from multiple options. Group with same `name` attribute.

## Other Useful Stuff

**Textarea** `<textarea>`  
Multi-line text input. Use `rows` and `cols` for size.

**Select** `<select>`  
Dropdown menu. Fill with `<option>` tags.

**Button** `<button>`  
Clickable button. More flexible than input submit.