# My Markdown Pandoc Resume

Markdown-to-anything resume/cover-letter generator!

You are like us; you hate keeping a resume. You also want to separate content and presentation (albeit as much as possible). Don't worry, we've done some styling for you! Just worry about writing in markdown and your resume will be set. 
You can git track it too! So when we inevitably get replaced by AI, that fast-food job you had from 7 years ago, will be important for getting you that next slave job.

The process is *fairly* simple.



## Usage:

Edit contents of resume.md:

    $ [ed/nano/vim/sublime] resume/resume.md
    $ make

Use templating for cover-letter:

    $ cd cover-letter/content
    $ [ed/nano/vim/sublime] arguments
    $ ./printletter > ../letter.md
    $ make

Note: The cover letter requires you edit the variables in the arguments file that it sources from.

## Dependencies:
* [Pandoc](https://pandoc.org/)
* [Wkhtmltopdf](https://wkhtmltopdf.org/)
* [CSS Knowledge](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [Markdown Knowledge](https://pandoc.org/MANUAL.html#pandocs-markdown)


## Benefits
1) *Version Control*. You track your resume via git/github! Say goodbye to the days where you had to remember all of your past achievements. Git will do that for you.
2) *Work-Flow*. You'll never have to update multiple things. It's all right here. Mkd-> HTML,PDF,DOCX
3) *CSS Styling*. Yes it's painful, but it's **_MUCH_** better than dealing with LaTex Template programming has. If you disagree, there are good [ LaTex/ConText templates ](https://github.com/jgm/pandoc/wiki/User-contributed-templates) for these kind of things.


## Installation
This project relies on [Pandoc](https://pandoc.org/), the swiss army knife conversion tool and [Wkhtmltopdf](https://wkhtmltopdf.org/), a way to create PDF's using a headless webpage.

* To install [Pandoc](https://pandoc.org/installing.html):
    - On Mac OSX use [brew package manager](https://brew.sh/)! -> ` brew install pandoc`
    - Windows Users use [chocolatey package manager](https://chocolatey.org/) -> `choco install pandoc`
    - Linux Users -> Check installation page for your distro!
* [WKhtmltopdf](https://wkhtmltopdf.org/downloads.html)
    - Mac OSX -> ` brew cask install wkhtmltopdf`
    - Windows Users -> Install from source!
    - Linux Users -> Check installation page for your distro!

#### Special Thanks
- My mom
- The inspiration from this simple [ MakeFile ](https://github.com/chmduquesne/resume/blob/master/Makefile).
