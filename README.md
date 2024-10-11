# Python setup

First of all, it requires `python3` and `pip3` or `pipenv` to be installed.  
```shell
$ git clone https://github.com/lorenzodifuccia/safaribooks.git
Cloning into 'safaribooks'...

$ cd safaribooks/
$ pip3 install -r requirements.txt

OR

$ pipenv install && pipenv shell
```  

The program depends of only two **Python _3_** modules:
```python3
lxml>=4.1.1
requests>=2.20.0
```

# Auth setup

```
One fast way to get the cookie:
Paste these code into Console of web inspector (F12) in firefox or chrome to get cookie, then paste into cookies.json
var output = {};document.cookie.split(/\s*;\s*/).forEach(function(pair) {pair = pair.split(/\s*=\s*/);output[pair[0]] = pair.splice(1).join('=');});console.log(JSON.stringify(output));
```
  
# Usage

```shell
$ python3 safaribooks.py XXXXXXXXXXXXX
```

The ID is the digits that you find in the URL of the book description page:  
`https://www.safaribooksonline.com/library/view/book-name/XXXXXXXXXXXXX/`  
Like: `https://www.safaribooksonline.com/library/view/test-driven-development-with/9781491958698/`  
