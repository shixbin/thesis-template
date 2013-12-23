LaTeX template for SJTU bachelor thesis
=======================================

Features
--------
- Header, footer, and margins
- Title page
- Table of contents
- Chapter and section title style
- Table and figure caption style
- Equation label style
- Bibliography and citation style

Usage
-----

    $ cd ~
    $ git clone git://github.com/stfairy/thesis-template.git
    $ git clone git://github.com/stfairy/thesis-bootstrap.git thesis
    $ cd thesis
    $ rm -rf .git
    $ ./link-templates
    $ make

You can add `thesis` to your version control system to track your own changes.
Changes to the thesis template can be pulled from `thesis-template` directory.

If you use a different location for `thesis-template`, modify `link-template` accordingly.

Prepare the following files in directory `thesis/body`.
- config.tex
- abstract.tex
- main.tex
- bibs.tex
- ack.tex

`\cite` is redefined to generate two citation formats:
- For the required citation format of "([n], Author, Year: Page.)", use `\cite[Page]{Name}` (e.g. `\cite[24]{JaffarYZ07}`).
- For inline text citation format of "Author (Year)", use `\cite{Name}` as normal (e.g. `\cite{JaffarYZ07}`).

Source code listings should be less than 70 columns in width for best display quality.

License
-------

    Copyright © 2013 Xiao Jia <me@xiao-jia.com>
    This work is free. You can redistribute it and/or modify it under the
    terms of the Do What The Fuck You Want To Public License, Version 2,
    as published by Sam Hocevar. See the COPYING file for more details.
