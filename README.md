# QL-dom

QL-dom is a library that helps beginner coders get started with DOM manipulation. QLdev is similar to jQuery in the way that it makes development simpler and quicker however it is not designed to be applied to development projects as it has limited capabilities. This library allows for students to use multiple different types of input in JavaScript and handles basic DOM (Document Object Model) modifications  
and manipulation in a very simple and straightforward way all in JavaScript. This allows for students to learn the basics of JavaScript while allowing basic use of more advanced functions to create basic working applications. The following are instructions for beginners on how to setup the QL-dom library, and use it. If you are a more advanced user you should understand the following quite easily, the library is a class that you will be linking to your HTML page and instantiating an object in your main JS file.

**Make sure all scripts other than QL-dom have the defer attribute.**

### INTRO

This git repo has the beginnings of a QL-dom project and file structure, it is very similar to the file structure of other features of the QL-dev framework. The library itself resides in the lib directory called QL-dom.js, however the file structure allows for you to start working on a website right out of the gate, simply open the index.html file in your browser and write your code in the app.js file, and you are ready to go!

# Use

**All created elements and fields are added to the bottom of the body.**  

**! = optional parameter**


### OUTPUT  

```javascript
print(text, !id);
```
creates a "p" element with the content of the text parameter, with or without an id attribute.  

```javascript
break(!id);
```  
Creates a "br" tag with or without an id attribute.  

```javascript
space(!size, !id);
```
This function allows you to make a space in your code to make it look better. You can give it a size in pixels and an id, or just a size, or nothing at all and will create your space with a default size of 25 pixels.  

```javascript
edit(id, text);
```
Changes the display value of a "p" tag with the matching id attribute.

```javascript
clearValue(id);
```
This function will clear the value of an input field.  

```javascript
remove(id);
```
Removed the element with the matching id attribute.  

```javascript
hide(id);
```
Hides the element with the matching id attribute from the user.  

```javascript
show(id);
```
Shows hidden elements to the user after them being hidden with the hide() function matching the id attribute.  

#### STYLES  

```javascript
textColor(id, color);
```
changes the text color of the element with the matching id to the specified color.  

```javascript
backgroundColor(id, color);
```
changes the background color of the element with the matching id to the specified color.  

#### LOGICAL  
```javascript
exists(id);
```
Returns true if an element with a matching id attribute exists.  

```javascript
valueOf(id);
```
Returns the value of the element with the matching id attribute, or innerHTML vale of p tag.  

#### META  
```javascript
changeAttribute(id, attribute, value);
```
This function allows you to add any valid html attribute and its value to an element with a matching id, or change the attribute if it already exists.  

```javascript
removeAttribute(id, attribute, value);
```
This function allows you to remove any html attribute that has previously been assigned to an element.  

```javascript
changeClass(id, newClass);
```
This function will change an existing class or add a class to an element that does not have one, where the id matches the id attribute.  

```javascript
removeClass(id);
```
This function will remove the class attribute from the element where the id matches the id attribute.  

```javascript
changeId(id, newId);
```
This function will change the id of the element with the matching id attribute to the newId.  

```javascript
removeId(id);
```
This function will remove the id attribute from the element where the id matches the id attribute.  

#### INPUT  
```javascript
button(text, fcn, !id);
```
This function allows you to create a button and link a function to it. text being what text is displayed on the button, fcn being the function you are linking, and id being the id attribute you are assigning to the button element.  

```javascript
keyPress(key, function)
```
This function allows you to write a function and have it execute when the specified key is pressed.  

```javascript
textBox(id);
```
This function creates a text box with an id.  

```javascript
textArea(id, !r, !c);
```
This function allows you to create a text area, this area is much larger than a text field, if you only include one parameter (being the id) it will make the text area with the default size of 10X50 characters, but if you include the parameters (r and c) you can specify the number of rows and columns of characters.  

```javascript
radioButton(id, name, value);
```
This function allows you to create a radio button, which is like a checkbox, but you can only select one of the group. In order to specify the group the 'name' parameter must be the same as all of the other radio buttons in the group. Then when you use the QL.value(); function include one id from any of the radio buttons apart of the group.  

```javascript
checkBox(id, value);
```
This function allows you to create a check box giving it an id and a value, if the checkbox is selected the 'value' parameter will be the result, if the box is not checked it will have the value of null.
