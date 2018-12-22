# django-piston
Django Piston Community Fork

fix piston3 bug list

1: ...
   response = func(*args, **kwargs)
  File "python3.6/site-packages/piston3/resource.py", line 148, in __call__
    return actor()
TypeError: challenge() missing 1 required positional argument: 'request'
...

2: ...
    from piston3.emitters import Emitter
  File "python3.6/site-packages/piston3/emitters.py", line 22, in <module>
    from django.core.serializers.json import DateTimeAwareJSONEncoder
ImportError: cannot import name 'DateTimeAwareJSONEncoder'

...

3: ...
#PY3: hmac doesn't work with str
...
