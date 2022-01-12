# followEveryoneTwitter
automatically follow Everyone Twitter


1.go to https://twitter.com/ {put the username here of the person you want to follow }/following

for eg. https://twitter.com/Pratik_the_king/following



2.open developer tools by pressing CNTRL + SHIFT + I 
3.Click on console tab 
4.Paste the following code 

```


var aTags = document.getElementsByTagName("span");
var searchText = "Follow";
var found=[];

for (var i = 0; i < aTags.length; i++) {
  if (aTags[i].textContent == searchText) {
     aTags[i].click();
  }
}
```




scroll down a little let new following load reapeat  step 4 


note twitter block our attempt to follow after certain number of follow requests
per day max you can follow 400 accounts 
https://help.twitter.com/en/using-twitter/twitter-follow-limit
