# 百度logo爬虫代码
import requests

if __name__ == '__main__':
    target = 'http://www.baidu.com/img/bd_logo1.png?qua=high&where=super'
    rsp = requests.get(url=target)

    with open('a.png',"wb") as f:
        f.write(rsp.content)
    print(rsp.text)

