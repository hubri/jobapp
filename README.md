# My Markdown Pandoc Resume

markdown-to-anything resume/cover-letter generator


The process is *fairly* simple.

## Usage:

Edit contents of resume.md

    $ [ed/nano/vim/sublime] resume/resume.md
    $ make

Use templating for cover-letter

    $ cd cover-letter/content
    $ [ed/nano/vim/sublime] arguments
    $ ./printletter > ../letter.md
    $ make

## Dependencies:
* [Pandoc](https://pandoc.org/)
* [Wkhtmltopdf](https://wkhtmltopdf.org/)
* [CSS Knowledge](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [Markdown Knowledge](https://pandoc.org/MANUAL.html#pandocs-markdown)


## Benefits
1) *Version Control*. You can track your resume via git/github! Say goodbye to the days where you had to remember all of your past achievements. Git will do that for you.
2) *Work-Flow*. You'll never have to update multiple things. It's all right here. Mkd-> HTML,PDF,DOCX
3) *CSS Styling*. Yes it's painful, but it's **_MUCH_** better than dealing with LaTex Template programming has. If you disagree, there are good [ LaTex/ConText templates ](https://github.com/jgm/pandoc/wiki/User-contributed-templates) for these kind of things.


## Installation
* Pandoc
    - Mac OSX -> ` brew install pandoc`
    - Windows Users -> idk google it
    - Linux Users -> sudo-apt-get?
* WKhtmltopdf
    - Mac OSX -> ` brew cask install wkhtmltopdf`
    - Windows Users -> idk google it
    - Linux Users -> sudo-apt-get?

#### Special Thanks
- My mom
- This simple [ MakeFile ](https://github.com/chmduquesne/resume/blob/master/Makefile).
