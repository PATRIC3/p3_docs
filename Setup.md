# Sphinx Installation

## Install Sphinx
```
pip install Sphinx
```

## Install markdown support
```
pip install recommonmark
```
See more detail http://www.sphinx-doc.org/en/stable/markdown.html

## Install readthedoc theme
```
pip install sphinx_rtd_theme
```
See more detail https://github.com/rtfd/sphinx_rtd_theme

## Install newsfeed plugin
```
pip install sphinxcontrib-newsfeed
```

# Local setting

```
# nginx conf

server {
	listen 80;
	server_name docs.patric.local;
	root /p3_docs/docroot/_build/html;
}
```

Add record for docs.patric.local in `/etc/hosts`
```
127.0.0.1	localhost
127.0.0.1	docs.patric.local
```