# Roam Research quick capture bookmarklet
A simple bookmarklet to capture text from a webpage to Roam Research.

You can use or adapt the code below or simple drag and drop this link to your bookmarks/favorites bar on you browser.

```
javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=__'+encodeURIComponent(d)+'__ — via ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+')#quick-capture','Roam','toolbar=no,width=700,height=350'));
```

<a href="javascript:q%3Dlocation.href%3Bif%28document.getSelection%29%7Bd%3Ddocument.getSelection%28%29%3B%7Delse%7Bd%3D%27%27%3B%7D%3Bp%3Ddocument.title%3Bvoid%28open%28%27https%3A%2F%2Froamresearch.com%3Ftext%3D__%27%2BencodeURIComponent%28d%29%2B%27__%20%E2%80%94%20via%20%5B%27%2BencodeURIComponent%28p%29%2B%27%5D%28%27%2BencodeURIComponent%28q%29%2B%27%29%23quick-capture%27%2C%27Roam%27%2C%27toolbar%3Dno%2Cwidth%3D700%2Cheight%3D350%27%29%29%3B">Capture to Roam</a>

## How to use

The bookmarklet uses the Mobile Quick Capture url integration (https://roamresearch.com/#/app/help/page/07-02-2020).

You can highlight a line of paragraph on a webpage and click the bookmarklet. A window popup will show you the same UI than on a mobile. You can add as many highlights or bookmarks as you want. 

To sync and see the captured text and url in Roam, you have to reload your app. A message asking if you want to sync the captured text will show.

This bookmarlet is adapted from the Pinboard bookmarklet.
