# How to deploy MKDOCS Project

## How to create new mkdocs project
<pre><code class="shell">C:\Users\sudhe>py -m mkdocs new sudheer</code></pre>
INFO    -  Creating project directory: sudheer

INFO    -  Writing config file: sudheer\mkdocs.yml

INFO    -  Writing initial docs: sudheer\docs\index.md

## How to run on localhost

<pre><code class="shell">C:\Users\sudhe>cd sudheer</code></pre>

<pre><code class="shell">C:\Users\sudhe\sudheer>py -m mkdocs serve</code></pre>
INFO    -  Building documentation...

INFO    -  Cleaning site directory

INFO    -  Documentation built in 0.38 seconds

INFO    -  [17:55:37] Watching paths for changes: 'docs', 'mkdocs.yml'

INFO    -  [17:55:37] Serving on http://127.0.0.1:8000/

INFO    -  [17:55:43] Browser connected: http://127.0.0.1:8000/

INFO    -  Shutting down...

## How to build code

<pre><code class="shell">C:\Users\sudhe\sudheer>py -m mkdocs build</code></pre>
INFO    -  Cleaning site directory

INFO    -  Building documentation to directory: C:\Users\sudhe\sudheer\site

INFO    -  Documentation built in 0.09 seconds

## Push code into github

<pre><code class="shell">C:\Users\sudhe\sudheer>echo "# sudheer.github.io" >> README.md</code></pre>

<pre><code class="shell">C:\Users\sudhe\sudheer>git init</code></pre>
Initialized empty Git repository in C:/Users/sudhe/sudheer/.git/

<pre><code class="shell">C:\Users\sudhe\sudheer>git add . -A</code></pre>
warning: in the working copy of 'site/404.html', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/css/base.css', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/css/bootstrap.min.css', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/css/font-awesome.min.css', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/fonts/fontawesome-webfont.svg', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/index.html', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/js/base.js', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/js/bootstrap.min.js', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/js/jquery-3.6.0.min.js', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/search/lunr.js', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/search/main.js', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/search/worker.js', LF will be replaced by CRLF the next time Git touches it

warning: in the working copy of 'site/sitemap.xml', LF will be replaced by CRLF the next time Git touches it

<pre><code class="shell">C:\Users\sudhe\sudheer>git commit -m "first commit"</code></pre>
[master (root-commit) a94e6ef] first commit

 24 files changed, 7339 insertions(+)

 create mode 100644 README.md

 create mode 100644 docs/index.md

 create mode 100644 mkdocs.yml

 create mode 100644 site/404.html

 create mode 100644 site/css/base.css

 create mode 100644 site/css/bootstrap.min.css

 create mode 100644 site/css/font-awesome.min.css

 create mode 100644 site/fonts/fontawesome-webfont.eot

 create mode 100644 site/fonts/fontawesome-webfont.svg

 create mode 100644 site/fonts/fontawesome-webfont.ttf

 create mode 100644 site/fonts/fontawesome-webfont.woff

 create mode 100644 site/fonts/fontawesome-webfont.woff2

 create mode 100644 site/img/favicon.ico

 create mode 100644 site/img/grid.png

 create mode 100644 site/index.html

 create mode 100644 site/js/base.js

 create mode 100644 site/js/bootstrap.min.js

 create mode 100644 site/js/jquery-3.6.0.min.js

 create mode 100644 site/search/lunr.js

 create mode 100644 site/search/main.js

 create mode 100644 site/search/search_index.json

 create mode 100644 site/search/worker.js

 create mode 100644 site/sitemap.xml

 create mode 100644 site/sitemap.xml.gz

<pre><code class="shell">C:\Users\sudhe\sudheer>git branch -M sudheer</code></pre>

<pre><code class="shell">C:\Users\sudhe\sudheer>git remote add origin https://github.com/SudheerKReddyG/sudheer.github.io.git</code></pre>

<pre><code class="shell">C:\Users\sudhe\sudheer>git push -u origin sudheer</code></pre>
Enumerating objects: 33, done.

Counting objects: 100% (33/33), done.

Delta compression using up to 8 threads

Compressing objects: 100% (30/30), done.

Writing objects: 100% (33/33), 606.38 KiB | 3.99 MiB/s, done.

Total 33 (delta 1), reused 0 (delta 0), pack-reused 0

remote: Resolving deltas: 100% (1/1), done.

To https://github.com/SudheerKReddyG/sudheer.github.io.git

 * [new branch]      sudheer -> sudheer

branch 'sudheer' set up to track 'origin/sudheer'.

## Deploy MKDOCS Project on git pages

<pre><code class="shell">C:\Users\sudhe\sudheer>py -m mkdocs gh-deploy</code></pre>
INFO    -  Cleaning site directory

INFO    -  Building documentation to directory: C:\Users\sudhe\sudheer\site

INFO    -  Documentation built in 0.17 seconds

WARNING -  Version check skipped: No version specified in previous deployment.

INFO    -  Copying 'C:\Users\sudhe\sudheer\site' to 'gh-pages' branch and pushing to GitHub.

Enumerating objects: 29, done.

Counting objects: 100% (29/29), done.

Delta compression using up to 8 threads

Compressing objects: 100% (28/28), done.

Writing objects: 100% (29/29), 605.92 KiB | 3.69 MiB/s, done.

Total 29 (delta 1), reused 0 (delta 0), pack-reused 0

remote: Resolving deltas: 100% (1/1), done.

remote:

remote: Create a pull request for 'gh-pages' on GitHub by visiting:

remote:      https://github.com/SudheerKReddyG/sudheer.github.io/pull/new/gh-pages

remote:

To https://github.com/SudheerKReddyG/sudheer.github.io.git

 * [new branch]      gh-pages -> gh-pages

INFO    -  Your documentation should shortly be available at: https://SudheerKReddyG.github.io/sudheer.github.io/