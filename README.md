Sheep Skin
==========

Sheep Skin is a document authoring utility.  It allows you to write your
document in Markdown and then compile it to HTML, Latex (PDF) and epub.  It's
especially useful for writing long, multi-section documents (such as books or
reports).  It uses Pandoc to parse your Markdown.

How it works
------------

When you invoke the `sheepskin` command, it will create a project directory
structure for you.  From then on, you don't need that command.  The project
contains a `Makefile` which does the rest.  You can customize the CSS, HTML and
Latex templates.

Usage
-----

1.  Download the `sheepskin` file and place it on your `PATH`.
2.  Create a directory for your project.
3.  Run `sheepskin`.  It will ask you some questions and create your project.
4.  Your text should live in the `src/` directory.  Chapters will be ordered
    alphabetically.
5.  Compile a version using the provided `Makefile`.
    * `make web`
    * `make latex`
    * `make epub`
6.  View the compiled output in `_build/`.

Requirements
------------

* Pandoc - [Installation instructions][1]

* LaTex - On Mac OSX, I'd recommend using [Basic Tex][2].  It's a very small
  package. You may need to install the `fontspect` package.

* [Kindle Previewer][3] (Optional) - This is for compiling the epub file to mobi and
  previewing.

License
-------

BSD, short and sweet.

[1]: http://johnmacfarlane.net/pandoc/installing.html
[2]: http://www.tug.org/mactex/2011/morepackages.html
[3]: http://www.amazon.com/gp/feature.html/?docId=1000765261
