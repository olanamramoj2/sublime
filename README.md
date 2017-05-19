# sublime

install sublime

install package-control:

Simple

The simplest method of installation is through the Sublime Text console. The console is accessed via the ctrl+` shortcut or the View > Show Console menu. Once open, paste the appropriate Python code for your version of Sublime Text into the console.

SUBLIME TEXT 3
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

This code creates the Installed Packages folder for you (if necessary), and then downloads the Package Control.sublime-package into it. The download will be done over HTTP instead of HTTPS due to Python standard library limitations, however the file will be validated using SHA-256.


ESSENTIAL SUBLIME TEXT PLUGINS FOR ALL DEVELOPERS
Also video previews, tips and tricks for Sublime Text Packages


SUBLIME TEXT
Introduction
As developers, we consume our time with code editors (or IDEs). Therefore there is a kind of inescapable emotional commitment. Just like some people we spend too much time with, code editors deserve attention, too.

I quite enjoy to be a developer with its all aspects, including trying to solve a problem, thinking how to write in an easier way, seeing a working example on browser, even finding right keywords to reach a specific solution on search engines. Most of these things can be made with code editors. For this reason, we need to make them realize what we demand and what we need. Thus, effective and faster code writing relies heavily on both developers and code editors' understanding each other very well.

I believe speed is the important thing for a developer if i set knowledge aside for a while. I regardlessly spend at least an hour with discovering and developing to automatize small works which do not take more than ten seconds but had to make them five times on a regular development day. For example, I spend half an hour for finding the right plugin, writing regular expressions, recording a macro, assigning a keyboard shortcut to it in order to make comment-out javascript console logs, which are not needed in a specific code block or function. it will not be a surprise to see this workflow as a waste of time by some of you. However, this would mean the person who does so is underestimating to make these small works over and over again which make someone lose focus. In addition, once you automatize such a series of work, the time you spent will be a profit of yours for the rest of your life.

Best Sublime Text Packages
We need plugins to fully customize Sublime Text rather than config customizations and tweaks. I am currently using Sublime Text version three but going to give alternatives for version two, too.

There are two different ways to install packages to Sublime Text.

First, you can download package repository zip file from package's github page then extract folder to Sublime Text Packages folder. (For Windows: {{ User name }}\AppData\Roaming\Subllime Text {{ version }}\Packages\ )

Second which is easier way, you can install through Sublime Text official Package Control manager. Navigate to page by clicking the link and grab the code that belongs to which Sublime version you have. Then, go back to Sublime Text window and paste copied code to Sublime Text Console (ctrl+"). You need to restart Sublime Text after installation complete. And lastly, open commands window, (ctrl + shit + p) then type Package Control: Install Package to install a package.

After you install a package, try to avoid making changes on package's default configuration file. Most packages will be installed as a single file on Sublime Text 3 and it does not let you modify default package configuration file. However,  all of the packages will be extracted to a folder on Sublime Text 2 and it's open for user's editing. Make changes as long as possible in packages' user config file. In this way, when packages or Sublime Text itself are upgraded, you will not lose any changes you made.

ESLINT
AdvancedNewFile

0:00

As it can be understood from its name, AdvancedNewFile makes possible to create new files and folders in Sublime Text. Without any need for Windows or Mac Navigator, you can create files or folders at any level of your project folder. In addition to its absolute and relative path option, you can also set default extension for newly created files.

Alignment

0:00

We align code snippets with Alignment package.

AngularJS

0:00

If you use Angular Js framework on your projects, this package would be what you need with SublimeCodeIntel package. SublimeCodeIntel cannot autocomplete Angular JS controllers' and modules' names in ng-*** attributes. With this package, you can autocomplete modules', controllers', factories' and services' variables by Rebuilt Search Index command. Package also makes possible to autocomplete all Angular JS attributes which start with ng-*** and snippets of Angular JS built-in functions like $http, $filter. 

Auto Semi-Colon

0:00

AutoSemiColon automatically ends line of CSS and Javascript files with ; semi-colon. If you do not want to get error while compressing js files, and more importantly to write a clean code, you should not miss semi-colon.

AutoFileName

0:00

AutoFileName is one of the top packages that I use mostly. It completes file names automatically. Generally, it autocompletes file names when cursor is between quotes, but I changed the configuration so that autocomplete triggers only with a key combination to avoid file names and variables mixed in the autocomplete pop-up list. 

ApacheConf.tmLanguage
ApacheConf.tmLanguage
ApacheConf.tmLanguage
Syntax highlight for Apache Configuration files. (.htaccess)

BracketHighlighter

0:00

It's one of my favourite packages of Sublime Text. It simply highlights your brackets. When cursor is between quotes, curly braces, parenthesis, it marks the beginning and the end of this part. While writing a complicated mathematical series or nested functions, this package helps you to see in which block the cursor is. It also covers advanced selection functions.

Case Conversion

0:00

We all have our own method of naming variables. If we write more than a couple languages, then it means we use more than a method of naming variables, like PascalCaseMethod, camelCaseMethod, snake_case_method ve kabab-case-method. With Case Conversion package, it is possible to pass through different naming methods with a single hotkey.

Color Highlighter
ColorHighlighter
ColorHighlighter
ColorHighlighter highlights your color values. It supports different kinds of color values like hex, rgb, rgba, hsl, hsla. It also highlights less and sass color variables.

Console Wrap for JS

0:00

It is one of the most underestimated packages for Javascript Developers. This package adds your variables to the second line in console logs.

CSS Extended Completions

0:00

This is my favourite package while writing css styles wtih css preprocessors. CSS Extended Completions package indexes your .less and .scss (or .sass) and caches your mixins, variables, class or id names and autocompletes both on html and css. It autocompletes your less and sass mixins with mixin arguments. It also supports emmet completions and gets your css classes on popup window. If you use common css patterns or mixins just like me, this package can index predefined folder path content on Sublime Text launch. Addition to these features, it searches stylesheet link tags on html files and indexes them, too. This feature is disabled on default. You have to make few adjustment on package configuration file to enable it.

DocBlockr
DocBlockr
DocBlockr
DocBlockr documents your code blocks and functions. It automatically makes entries for function arguments, variables' types and descriptions.

Emmet
Emmet Official Documentation says:

Basically, most text editors out there allow you to store and re-use commonly used code chunks, called “snippets”. While snippets are a good way to boost your productivity, all implementations have common pitfalls: you have to define the snippet first and you can’t extend them in runtime.

Emmet takes the snippets idea to a whole new level: you can type CSS-like expressions that can be dynamically parsed, and produce output depending on what you type in the abbreviation. Emmet is developed and optimised for web-developers whose workflow depends on HTML/XML and CSS, but can be used with programming languages too.
Emmet is the most downloaded package of Sublime Text with 2,2 million downloads on Sublime Text Package Community. It replaced ZenCoding a long time ago and still is the most popular package. There is no need to explain it, just take a look at Official Documentation. 

Gist

0:00

Gist is a part of Github which you can share your snippets or code blocks with both public and private. This extension makes possible for you to reach your gists directly via Sublime Text. You can create, modify, delete or view all your Gists only with a few commands.

Grunt

0:00

Grunt is node based task runner system just like Gulp. This package allows you to run grunt commands within Sublime Text without touching terminal window.

HTML Nest Comments

0:00

Sublime text cannot recognize already commented out html codes in selection. Moreover, it tries to enter the html comment markup only at the beginning and the end of the selection. This package comments out html code blocks which has been already commented out html code.  

HTML5
This package adds new HTML5 tag completion to Sublime Text, like section, main, header, footer, figure.

Inc-Dec-Value

0:00

This Sublime Text package is not known well by developers. Just like Emmet does, Inc-Dec-Value makes possible to modify numbers incremented and decremented by 0.1, 1, 10, 100. It also converts color formats from one to another, like hex, rgb, rgba, hsl, hsla. The most important feature of Inc-Dec Value is to pass through between pre-defined word arrays. For example, I defined all javascript and CSS opposite values in arrays, like fadeIn / fadeOut, true / false, show / hide, static / relative / absolute / fixed and next / prev.

jQuery

0:00

jQuery is the most popular javascript library and this package adds jQuery functions' completion feature to Sublime Text with callbacks options.

LESS
LESS
LESS
If you use less.js as CSS Preprocessor, this package adds syntax highlight feature to .less files. It also completes built-in LESS functions, like fadein, darken, desaturate, data-uri.

Local History

0:00

It is one of my favorites, too. You can think Local History as a local version system just like Git. It backs up currently editing file on a folder every time you hit ctrl + s. It also compares backed up files with the current one just like Git diff command.

Monokai Extended
Monoka Extended is an alternate and advanced version of Sublime Text's default color scheme Monokai.

Quick File Open
Quick File Open
Quick File Open
This package makes possible to reach pre-defined files with a single hotkey.

Random Everything

0:00

Random Everything is not much known package of Sublime Text by developers. This package generates random data including date (DD/MM/YYYY formatted), integers on a specific range, random letters, random paragraph, UUID, url, random word, e-mail address, human name, human surname, human name and surname, hex formatted color, IPv4 address, IPv6 address and random value that both includes letters and numbers. It is a very handy package and its usage area depends on your imagination. You can generate html tables with logical values within few seconds. 

RegReplace

0:00

RegReplace package handles predefined regex replaces for you. It includes few regex replace functions already like removing comments on html file, trimming white spaces (Sublime Text has a built in method for this purpose on save) and removing HTML5 deprecated tags. For example; i created a regexp replace function to comment-out console logs and vice versa on javascript files. There is no limit that you can do with it.

SASS
SASS
SASS
If you use SASS as CSS Preprocessor, this package adds syntax highlight feature to .scss and .sass files. It also completes built-in SASS functions, like @mixin, @include and @if @else statements.

SFTP

0:00

Filezilla is a very diffucult and long way to reach remote files. I often see that developers launch Filezilla to upload files to local server. SFTP Package makes possible to edit, delete, browse, sync, upload and download files on remote server. It is a one of the handy packages of Sublime Text.

SideBarEnhancements

0:00

Sublime Text Sidebar commands are quite limited and only handles simple actions. SideBarEnhancements package is one of the must installed packages of Sublime Text. It gains your Sidebar context menu a lot of enhancments. You can set "open with" command to specific extensions, like opening image files with Photoshop or open your html files with different browsers and assign a specific hotkey to these commands. It supports copy, cut or move between files and folder without touching file explorer. It also makes possible to copy file path, copy file name, search on a specific folder or show selected file on Windows Explorer.

StyleToken

0:00

StyleToken is one of the unknown of Sublime Text packages, too. It makes possible to focus different parts of code or word definition with different highlight styles.

SublimeCodeIntel
SublimeCodeIntel package turns your text editor to fully featured IDE. You have definitely install it for extended and advanced code completion on Sublime Text. With a new release of SublimeCodeIntel, you will notice the code completion logic reached higher level compare to previous version.

This package makes possible to autocomplete every single word definition on your project. It supports JavaScript, SCSS, Python, HTML, Ruby, Python3, XML, Sass, HTML5, Perl, CSS, Twig, Less, Node.js, TemplateToolkit and PHP completion predefined on config file.

SublimeLinter
SublimeLinter
SublimeLinter
SublimeLinter package simply lints your code. It supports PHP, Javascript, Java, CSS, HTML, HAML, Python, Ruby, Json, CoffeeScript, Google Closure, XML, React.js, Slim, Markdown, Go, Perl, C, C++, SQL, Twig, Bootstrap, Jade, LESS, SASS for now. If you want to notice your syntax errors on Sublime Text before browser, or more importantly write cleaner code, you must install SublimeLinter package to achieve your goal. SublimeLinter is a core package for linting, you must install additional packages for each language or framework to make linting process work.

SwapStrings

0:00

Let's assume that you have mixed two variable a file. For example, you accidently typed up instead of down, and typed down where you must type up. What is the fastest way to get over this problem? First, you replace up word with quite unique value, like hfjdhj34gj5h3. Then replace down word with up. And lastly, you replace hfjdhj34gj5h3 value with up. This package allows you to replace two variable or word with each other. It also change double quotes to single and single quotes to double within a selected code block or whole document.

Terminal
Terminal
Terminal
As a developer, we often use terminal to automatize our jobs through Bower, Grunt, Gulp, npm or node. Beside Sublime Text, some of the editors have built-in Terminal support just like Visual Studio and WebStorm. This package makes possible to open terminal window with a single hotkey and sets project root folder as base folder. It also sets currently opened file path as base folder, too.

Published by Ömer Aslanbakan on 14 October 2015

POPULAR POSTS

Less Space 
Responsive CSS Margin and Padding Helper Classes
No need to use media queries anymore with SASS and LESS
26 May 2015
Viewed 28443 times
Browser and Device specific CSS Styles with SASS and LESS mixins
Without 3rd party plugins with a single line of Javascript code
27 December 2015
Viewed 15088 times
Validate Turkish TC ID Number with Javascript
With 3 different validation method
27 February 2015
Viewed 7764 times
Print window dimensions with browser variables for responsive tests
No need to check from developer console
17 February 2015
Viewed 3774 times
POPULAR POSTS
33 Essential Sublime Text Plugins for All Developers
Less Space Responsive CSS Margin and Padding Helper Classes
Browser and Device specific CSS Styles with SASS and LESS mixins
Validate Turkish TC ID Number with Javascript
Print window dimensions with browser variables for responsive tests
BLOG CATEGORIES
HTML5
Javascript
CSS3
Sublime Text
jQuery
BLOG TAGS
HTML5
CSS3
Javascript
jQuery
LESS
 Copyright by Ömer Aslanbakan © 2017
           
