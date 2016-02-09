UnderStrap WordPress Theme Framework
===

Website: http://understrap.com

About
=
Basically I like the _s WordPress Starter Theme from Automattic and the grid Framework Bootstrap. Additionally I´am a huge SASS fan. Why don´t combine all these three things into a solid WordPress Theme Framework?
That´s what UnderStrap is (or will be...)

At the moment UnderStrap is in a very early stage. But if you wan´t feel free to use it for your own WordPress theme!

Basic Features
=
- Combines the _s WordPress Starter Theme PHP/JS files and Bootstrap´s HTML/CSS/JS
- Comes with Bootstrap (3.3.6) SASS source files and additional scss files. Nicely sorted and ready to add your own variables/customize the Bootstrap variables.
- Uses a single and minified CSS file for all the basic stuff
- Font Awesome Icon Font integrated (V 4.5.0): http://fortawesome.github.io/Font-Awesome/
- Comes with extra slider script - By owl.carousel (V 2.0.0-beta.2.4): http://www.owlcarousel.owlgraphic.com/
- Simple RTL file
- Jetpack ready
- WooCommerce support
- Child Theme ready (A basic starter Child Theme will be released in the future as a separate Repository)
- Translation ready

Starter Theme + HTML Framework = WordPress Theme Framework
=
The _s theme is a good starting point to develope a WordPress theme. But it is "just" a raw starter theme. Means it outputs all the WordPress stuff correctly but without any layout or design.
Why don´t add a well known and supported layout framework to have a solid, clean and responsive foundation? Thats where Bootstrap comes in.

Confused by all the CSS and SCSS files?
=
Some basics about the SCSS and CSS files comes with UnderStrap:
- The theme itself uses the style.css in the root directory just to identify the theme inside of WordPress. The file is not loaded by the theme and did not include any styles
- The theme.css file in /css/ subdirectory provides all styles. It is composed by five different SCSS sets and one variables file from /sass/theme.scss:

                  - 1 "theme/theme_variables";  // <--------- Add your variables into this file. Also add variables to overwrite Bootstrap or UnderStrap variables here
                  - 2 "../bower_components/bootstrap-sass/assets/stylesheets/bootstrap";  // <--------- All the Bootstrap stuff - Don´t edit this!
                  - 3 "understrap/understrap"; // <--------- Some basic WordPress stylings and needed styles to combine Boostrap and Underscores
                  - 4 "../bower_components/fontawesome/scss/font-awesome"; // <--------- Font Awesome Icon styles

                  // Any additional imported files //
                  - 5 "theme/theme";  // <--------- Add your styles into this file

- Don´t edit the files no. 2-4 files/filesets or you aren´t able to update it without overwriting your own work!
- Your design goes into: /sass/theme directory. Add your styles to the theme.scss file and your variables to the _theme_variables.scss. Or add other scss files into it and @import it into theme.scss

Installation
=
- Download the understrap folder
- Upload it into your WordPress installation subfolder here: /wp-content/themes/
- Login to your WordPress backend
- Go to Appearance -> Themes
- Activate the UnderStrap theme

How to use the build-in Widget Slider?
=
The frontpage slider is widget driven. Simply add more than one widget to widget position.
- Click on Appearance -> Widgets
- Add two or more widgets of any kind to widget area "Hero"
- Thats it
