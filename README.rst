
============
Django-Agora
============

.. image:: https://badge.fury.io/py/django-agora.svg
    :target: https://badge.fury.io/py/django-agora
    :alt: Agora

.. image:: https://travis-ci.org/raysandeep/django-agora.svg
   :target: https://travis-ci.org/raysandeep/django-agora
   :alt: Build Status

.. image:: https://badge.fury.io/gh/raysandeep%2Fdjango-agora.svg
    :target: https://badge.fury.io/gh/raysandeep%2Fdjango-agora
    :alt: Agora

Django-Agora is a Django app to help integrating Video Calling Feature Using Agoro.io .

Quick start
-----------

1. Add "agora" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'agora',
    ]

2. Import Agora views in your project urls.py like this::
    
    from agora.views import Agora
        
3. Include the agora view in your project urls.py like this::
    
    path('agora/',Agora.as_view(
        app_id='<APP_ID>',
        channel='<CHANNEL_ID>'
    )),

4. Visit http://127.0.0.1:8000/agora/ to participate in the Video Call.
