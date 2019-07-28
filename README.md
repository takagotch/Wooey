### wooey
---
https://github.com/wooey/wooey

```py
MIDDLEWARE_CLASSES = (
  'django.contrib.sessions.middleware.SessionMiddleware',
  'django.middleware.locale.LocaleMiddleware',
  'django.middleware.common.CommonMiddleware',
  'django.middleware.csrf.CsrfViewMiddleware',
  'django.contrib.auth.middleware.AuthenticationMiddleware',
  'django.contrib.auth.middleware.AuthenticationMiddleware',
  'django.contrib.messages.middleware.MessageMiddleware',
  'django.middleware.clickjacking.XFrameOptionsMiddleware',
  'django.middleware.security.SecurityMiddleware'
)

import argparse
import sys

parser = argparse.ArgumentParser(description="Find the sum of all the numbers below a certain number.")
parser.add_argument('--below', help='The number to find the sum of numbers below.', type=int, default=1000)

def main():
  args = parser.parse_args()
  s = sum((i for i in range(args.below)))
  print("Sum =", s)
  return 0
  
if __name__ == "__main__":
  sys.exit(main())
```

```sh
python manage.py runserver
celery -A your_project_name worker -c 1 --beat -l info
python manage.py runserver
```

```
```


