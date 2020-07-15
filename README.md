# Roam Research quick capture bookmarklet
A simple bookmarklet to capture text from a webpage to Roam Research.

```
javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=__'+encodeURIComponent(d)+'__ — via ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+')#quick-capture','Roam','toolbar=no,width=700,height=350'));
```

The bookmarklet uses the Mobile Quick Capture url integration (https://roamresearch.com/#/app/help/page/07-02-2020).

You can highlight a line of paragraph on a webpage and click the bookmarklet. A window popup will show you the same UI than on a mobile. You can add as many highlights or bookmarks as you want. 

To see the captured text and url in Roam, you have to reload your app. A message asking if you want to sync the captured text will show.

This bookmarlet is adapted from the Pinboard bookmarklet.
