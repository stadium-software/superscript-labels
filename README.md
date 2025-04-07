# Superscript Labels

When vertical space is at a problem, you can use this module to display a field label in Superscript above the field. 

![Superscript Labels](images/superscript-labels.png)

## Version

1.0 - initial

1.0.1 Updated Readme to 6.12+; Converted px to rem

# Setup

## Application Setup

1. Check the *Enable Style Sheet* checkbox in the application properties

## Page Setup

1. Drag a *Container* control into the page 
2. Add a class called "stadium-superscript-label" into the *Container* classes property
3. Drag a *Label* control into the *Container* control
4. Add the text you wish to show on the label into the text property
5. Drag a *CheckBoxList*, *DatePicker*, *DropDown*, *RadioButtonList*, *Textbox* or *UploadFile* control into the *Container* control

![Controls Setup](images/controls.png)

## CSS
The CSS below is required for the correct functioning of the module. Variables exposed in the [*css-file-variables.css*](css-file-variables.css) file can be [customised](#customising-css).

### Before v6.12
1. Create a folder called "CSS" inside of your Embedded Files in your application
2. Drag the two CSS files from this repo [*css-file-variables.css*](css-file-variables.css) and [*css-file.css*](css-file.css) into that folder
3. Paste the link tags below into the *head* property of your application
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file.css">
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file-variables.css">
``` 

### v6.12+
1. Create a folder called "CSS" inside of your Embedded Files in your application
2. Drag the CSS files from this repo [*css-file.css*](css-file.css) into that folder
3. Paste the link tag below into the *head* property of your application
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file.css">
``` 

### Customising CSS
1. Open the CSS file called [*css-file-variables.css*](css-file-variables.css) from this repo
2. Adjust the variables in the *:root* element as you see fit
3. Stadium 6.12+ users can comment out any variable they do **not** want to customise
4. Add the [*css-file-variables.css*](css-file-variables.css) to the "CSS" folder in the EmbeddedFiles (overwrite)
5. Paste the link tag below into the *head* property of your application (if you don't already have it there)
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file-variables.css">
``` 
6. Add the file to the "CSS" inside of your Embedded Files in your application

**NOTE: Do not change any of the CSS in the 'css-file.css' file**

## Upgrading Stadium Repos
Stadium Repos are not static. They change as additional features are added and bugs are fixed. Using the right method to work with Stadium Repos allows for upgrading them in a controlled manner. 

How to use and update application repos is described here: [Working with Stadium Repos](https://github.com/stadium-software/samples-upgrading)