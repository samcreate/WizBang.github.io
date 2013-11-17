![](https://raw.github.com/samcreate/WizBang/master/images/wiz_bang_icon60x60.png)WizBang
=======

 

Converts Layer names to optimized web images automatically 

Turns a photoshop layer named: "{retina:true}logo.mini.png" into a transparent web optimized PNG named "logo.mini.png" and creates 2x retina version named "logo.mini@2x.png" in a folder that you specify... All with correct dimensions and flattened layers styles. 

Layer name into image! Behold!

![](https://raw.github.com/samcreate/WizBang/master/images/layer.examples.png) 


### First, download the script:

[Download export_NameToFile.jsx](https://raw.github.com/samcreate/WizBang/master/export_NameToFile.jsx)

### Second, Install the Photoshop Script
1. Close Photoshop if it is open.
2. Copy the script and its ‘Scripts Only’ folder to the Scripts folder in your Photoshop installation directory.
  - On Windows: C:\Program Files\Adobe\Photoshop CS[x]\Preset\Scripts.
  - On a MAC  : Applications > Photoshop CS[x] -> Presets -> Scripts.
3. Open Photoshop.
4. The script will now appear on the File > Scripts menu and can be run from here at any time.


### Documentation:

Below are the options you can add to the layer name for finer control of the exported image. Each example is showing one parameter but note that you can add as many applicalble parameters as you want, per layer name. 

#### JPG:

basic 
```javascript
name_of_image.jpg
```

quality (number in percent)
```javascript
{quality:80} name_of_image.jpg
```

retina (boolean)
```javascript
{retina:true} name_of_image.jpg
```

width (number)
```javascript
{w:400} name_of_image.jpg
```

height (number)
```javascript
{h:400} name_of_image.jpg
```

=======
#### PNG:

basic 
```javascript
name_of_image.png
```

png8 (boolean) (exports a png8 image)
```javascript
{png8:true} name_of_image.png
```

matte (hex color)
```javascript
{matte:'#ff0000'} name_of_image.png
```

retina (boolean)
```javascript
{retina:true} name_of_image.png
```

width (number)
```javascript
{w:400} name_of_image.png
```

height (number)
```javascript
{h:400} name_of_image.png
```

=======
#### GIF:

basic 
```javascript
name_of_image.gif
```

matte (hex color)
```javascript
{matte:'#ff0000'} name_of_image.gif
```

width (number)
```javascript
{w:400} name_of_image.gif
```

height (number)
```javascript
{h:400} name_of_image.gif
```
=======

