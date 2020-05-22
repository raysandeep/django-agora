
==============
Django-AgoraVC
==============

Django-Agora is a Django app to help integrating Video Calling Feature Using Agoro.io .

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "agora" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'agora',
    ]

2. Include the agora URLconf in your project urls.py like this::

    path('agora/',Agora.as_view(
        app_id='<APP_ID>',
        channel='<CHANNEL_ID>'
    )),

3. Visit http://127.0.0.1:8000/agora/ to participate in the Video Call.