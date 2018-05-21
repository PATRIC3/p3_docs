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

## Install plugins
```
pip install sphinxcontrib-newsfeed
pip install sphinxcontrib-spelling
```

# Local setting
Install nginx and config like below. Set document root accordingly.
```
# nginx conf

server {
	listen 80;
	server_name docs.patric.local;
	root /p3_docs/docroot/_build/html;

        # to avoid Cross-Origin Request Blocked error
        location / { 
          if ($request_method = 'OPTIONS') {
             add_header 'Access-Control-Allow-Origin' '*';
             add_header 'Access-Control-Allow-Methods' 'GET, OPTIONS';
             add_header 'Access-Control-Allow-Headers' 'Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type,Content-Range,Range';
             return 204;
          }
          if ($request_method = 'GET') {
             add_header 'Access-Control-Allow-Origin' '*';
             add_header 'Access-Control-Allow-Methods' 'GET, OPTIONS';
          }
        }
}
```

Add record for docs.patric.local in `/etc/hosts` with sudo
```
127.0.0.1	localhost
127.0.0.1	docs.patric.local
```
