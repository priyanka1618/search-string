# search-string
import requests 
wikipedia2 = requests.get('https://www.quora.com/')
page2 = wikipedia2.text
#print(page2)
album_title = page2[page2.find('<title>') +7 : page2.find('</title>')]
print(album_title)
