# Welcome to the cms-onebyteoftravel!

1. Django-CMS
> `Django 1.11`
> `python 2.7`
> `djangocms-blog==0.9.7`
> `django-cms==3.5.2`
2. Google App Engine
> `Standard Enviroment`
<pre>
runtime: python27
api_version: '1'
env: standard
threadsafe: true
instance_class: F1
libraries:
  - name: pytz
    version: '2017.2'
  - name: six
    version: 1.9.0
  - name: MySQLdb
    version: 1.2.5
  - name: django
    version: '1.11'
  - name: ssl
    version: 2.7.11
  - name: pytz
    version: '2017.3'
  - name: PIL
    version: 1.1.7
  - name: lxml
    version: 3.7.3
handlers:
  - url: '/static/(.*)'
    application_readable: false
    static_files: "static/\\1"
    require_matching_file: false
    upload: 'static/.*'
  - url: '.*'
    script: onebyteoftravel.wsgi.application
automatic_scaling:
  min_idle_instances: automatic
</pre>
3. SQL Instance : Google Cloud Platform

> `db-f1-micro`
> `1 vCPUs`, `memory 614.4 MB.`

4. Domain mapping & SSL certificates
> `Google managed`

5. Domain Name Registration
> `Gandi.net`

6. Google Analytics
> `gtag.js`

7. Social Share
> `LinkedIn`
> `Google+`
> `Facebook`
> `Twitter`

8. Sitemap XML
> `django.contrib.sitemaps`
> `http://onebyteoftravel.com/sitemap.xml`

9. RSS feed
> `google feedburner`
> `http://feeds.feedburner.com/OneByteOfTravel`

