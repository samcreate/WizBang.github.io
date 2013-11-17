WizBang
=======


Converts Layer names to optimized web images automatically 

Turns a photoshop layer named: "{retina:true}logo.mini.png" into a transparent web optimized PNG named "logo.mini.png" and creates 2x retina version named "logo.mini@2x.png" in a folder that you specify... All with correct dimensions and flattened layers styles. 

Layer name into image! Behold!

![](https://raw.github.com/samcreate/WizBang/master/images/layer.examples.png) 


### Installing a Photoshop Script
1. Close Photoshop if it is open.
2. Copy the script and its ‘Scripts Only’ folder to the Scripts folder in your Photoshop installation directory.
  - On Windows: C:\Program Files\Adobe\Photoshop CS[x]\Preset\Scripts.
  - On a MAC  : Applications > Photoshop CS[x] -> Presets -> Scripts.
3. Open Photoshop.
4. The script will now appear on the File > Scripts menu and can be run from here at any time.
 
### Running a Photoshop Script without Installing
1. Open Photoshop.
2. Select File -> Scripts -> Browse and navigate to the "export_NameToFile.jxs" file.
 
### Running a script from a shortcut
Many applications have shortcuts or hot keys to allow you to access frequently used functionality faster. If you install your script to the File -> Scripts menu you can allocate a keyboard shortcut to run the script using the instructions below.

1. Launch the keyboard shortcuts dialog by clicking Edit > Keyboard Shortcuts.
2. Under "Application Menu Command" open the entry for "File".
3. Scroll down, past "Scripts" until you see the name of your script.
4. Click the blank area for the script's shortcut.
5. Type the required shortcut. You can choose any combination of keystrokes as long as the following two points are met:
  - You must include "Ctrl" or a function key.
  - Do not use "Alt". This will launch the script in ‘Debug’ mode, rather than run it properly.
6. When finished, click OK.


### Documentation:

Below are the options you can add to the layer name for finer control of the exported image. Each example is showing one parameter but note that you can add as many applicalble parameters as you want, per layer name. 

#### JPG:

basic 
```php
name_of_image.jpg
```

quality (number in percent)
```php
{quality:80} name_of_image.jpg
```

retina (boolean)
```php
{retina:true} name_of_image.jpg
```

width (number)
```php
{w:400} name_of_image.jpg
```

height (number)
```php
{h:400} name_of_image.jpg
```

=======
#### PNG:

basic 
```php
name_of_image.png
```

png8 (boolean) (exports a png8 image)
```php
{png8:true} name_of_image.png
```

matte (hex color)
```php
{matte:'#ff0000'} name_of_image.png
```

retina (boolean)
```php
{retina:true} name_of_image.png
```

width (number)
```php
{w:400} name_of_image.png
```

height (number)
```php
{h:400} name_of_image.png
```

=======
#### GIF:

basic 
```php
name_of_image.gif
```

matte (hex color)
```php
{matte:'#ff0000'} name_of_image.gif
```

width (number)
```php
{w:400} name_of_image.gif
```

height (number)
```php
{h:400} name_of_image.gif
```
=======

