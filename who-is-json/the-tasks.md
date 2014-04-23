# The Tasks

What Grunt can do is automate things we would do anyways when developing websites. It doesn't sound like much but let me give you an example.

Grunt automates things like watching for clean code in your HTML, CSS or JS files. It can convert LESS to CSS and then minify the output CSS file and it can concatenate Javascript files and uglify them afterwards.

It could even take images you placed in a directory, compress them with a lossless compression-tool, create two new directories afterwards, put two version of the original image with different sizes in those folders, where one of them is cropped by 20 pixels on top and right and finally clear the original directory from the source file.

Still doesn't sound like much? Oh, there are so many more things Grunt is capable of but let's not get distracted and start with the little things.

Simple tasks you would do manually, automated by Grunt - and here are the tasks we will use in this course:

## [HTMLhint](https://github.com/yaniswang/grunt-htmlhint) by Yanis Wang

HTMLhint is analizing your HTML. You can define how strict the hinting will be and we will do that in the gruntfile later on.

## [LESS](https://github.com/gruntjs/grunt-contrib-less)

This task watches for your LESS files and creates a valid CSS file out of them.

## [Autoprefixer](https://github.com/nDmitry/grunt-autoprefixer) by Dmitry Nikitenko

Here we have an amazing and powerful task at our hands. The autoprefixer will take your CSS file and put prefixes where needed and takes them away where browsers support the attributes or selectors you defined. It is taking the [caniuse.com](www.caniuse.com) database to add or subtract prefixes to your CSS.

On top you can define in the gruntfile how many versions back and from what percentage of marketshare you want to support a browser. You could even turn to specific browsers (I'm not going to tell you which Microsoft browser I'm talking about ... oops) and support their special needs.

## [CSSmin](https://github.com/gruntjs/grunt-contrib-cssmin)

Nothing too surprising here. This task is taking CSS files and compresses them into a one lined, humanly unreadable version. You can define a name for those minified files in your gruntfile.

## [Watch](https://github.com/gruntjs/grunt-contrib-watch)

This one is also quite handy as it runs all the above tasks (or only one of them) when specific files change. For example you could change one attribute in one less file. The watch task will then run the specified tasks for less files, like creating a CSS file out of them.

Let's go on and tell the tasks what, what not and most importantly how to do what they are good at.