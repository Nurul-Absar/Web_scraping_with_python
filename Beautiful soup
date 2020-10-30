import urllib.request as urllib2
from bs4 import BeautifulSoup
n=int(input())
s=0
for i in range(1,n+1):
  root_address="https://www.rottentomatoes.com/m/deadpool/reviews?type=&sort=&page=i"
  page=urllib2.urlopen(root_address)
  soup = BeautifulSoup(page, 'html.parser')
#print(soup.prettify()) show all html code
  reviews=soup.find_all('div',attrs={'class':'the_review'})
 
  for j in reviews:
     print("Review:",j.get_text(), "\n")
 
  for k in range(len(reviews)):
    s=s+1
    print("Total Review:", s)


