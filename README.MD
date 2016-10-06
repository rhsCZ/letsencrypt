get python version `$ python -V`
install python 2 requirements for hook cloudflare
```
$ pip install -r ~/workspace/letsencrypt/cloudflare-hook/requirements-python-2.txt
```
config for cloudflare hook
```
$ export CF_EMAIL='user@example.com'
$ export CF_KEY='K9uX2HyUjeWg5AhAb'
```
if you cant execute executable file dehydrated so run
```chmod +x dehydrated```
and run command
```./dehydrated -c -d example.com -t dns-01 -k '~/workspace/letsencrypt/cloudflare-hook/hook.py' -f '~/workspace/letsencrypt/config-letsencrypt'```
