get python version `$ python -V`
install python 2 requirements for hook cloudflare
```
$ pip install -r ~/workspace/letsencrypt/cloudflare-hook/requirements-python-2.txt
```
if error run
```
sudo apt-get install build-essential autoconf libtool pkg-config python-opengl python-imaging python-pyrex python-pyside.qtopengl idle-python2.7 qt4-dev-tools qt4-designer libqtgui4 libqtcore4 libqt4-xml libqt4-test libqt4-script libqt4-network libqt4-dbus python-qt4 python-qt4-gl libgle3 python-dev
```
config for cloudflare hook
```
$ export CF_EMAIL='user@example.com'
$ export CF_KEY='K9uX2HyUjeWg5AhAb'
```
if you cant execute executable file dehydrated so run
```
$ chmod +x dehydrated
```
and run command
```
$ ./dehydrated -c -d example.com -t dns-01 -k '~/workspace/letsencrypt/cloudflare-hook/hook.py' -f '~/workspace/letsencrypt/config-letsencrypt'
```
