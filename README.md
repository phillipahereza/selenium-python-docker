## Selenium Python Docker

An docker image for functional testing inspired by [Test Driven Development with Python](https://www.obeythetestinggoat.com) by Harry J.W Percival


### Usage
```
docker pull ahereza/python-selenium

docker run -it ahereza/python-selenium sh
>>> from selenium import webdriver
>>> chrome_options = webdriver.ChromeOptions()
>>> chrome_options.add_argument('headless')
>>> chrome_options.add_argument('no-sandbox')
>>> chrome_options.add_argument('disable-gpu')
>>> browser = webdriver.Chrome(options=chrome_options)
>>> browser.get("http://google.com")
```