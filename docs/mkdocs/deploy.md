# How to Install Python and Setup MKDOCS

## Install Python

<pre><code class="shell">https://www.python.org/downloads/</code></pre>

## Check the Python version

<pre><code class="shell">py --version</code></pre>

## Install Python plugin visual studio code

<pre><code class="shell">python -> Install</code></pre>

## Install Plugins for MKDOCS

<pre><code class="shell">python -m pip install mkdocs --trusted-host=pypi.python.org --trusted-host=pypi.org --trusted-host=files.pythonhosted.org --user</code></pre>

<pre><code class="shell">python -m pip install --upgrade pip --trusted-host=pypi.python.org --trusted-host=pypi.org --trusted-host=files.pythonhosted.org --user</code></pre>

<pre><code class="shell">python -m pip install mkdocs-material --trusted-host=pypi.python.org --trusted-host=pypi.org --trusted-host=files.pythonhosted.org --user</code></pre>

<pre><code class="shell">python -m pip install mkdocs-git-version-date-localized-plugin --trusted-host=pypi.python.org --trusted-host=pypi.org --trusted-host=files.pythonhosted.org --user</code></pre>

## Create new MKDOCS Project

<pre><code class="shell">py -m mkdocs new <Project Name></code></pre>

## Start the app on localhost

<pre><code class="shell">py -m mkdocs serve</code></pre>

## Build the code

<pre><code class="shell">py -m mkdocs build</code></pre>

## Deploy code on Pages

<pre><code class="shell">py -m mkdocs gh-deploy</code></pre>