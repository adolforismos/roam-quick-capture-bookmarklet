# Roam Research quick capture bookmarklet
A simple bookmarklet to capture text from a webpage to Roam Research.

You can use or adapt the code below or simple drag and drop this link to your bookmarks/favorites bar on you browser.

This is in the format of:

_quote_ — via [link to page](https://google.com)

```
javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=__'+encodeURIComponent(d)+'__ — via ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+') [[Quotes]]#quick-capture','Roam','toolbar=no,width=700,height=350'));
```

<a href="javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=__'+encodeURIComponent(d)+'__ — via ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+') [[Quotes]]#quick-capture','Roam','toolbar=no,width=700,height=350'));">Capture to Roam</a>

This just grabs the title and link in markdown.

```
javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=['+encodeURIComponent(p)+']('+encodeURIComponent(q)+') [[link]]#quick-capture','Roam','toolbar=no,width=700,height=350'));
```
<a href="javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=['+encodeURIComponent(p)+']('+encodeURIComponent(q)+') [[link]]#quick-capture','Roam','toolbar=no,width=700,height=350'));">Title/Link to Roam</a>

This is to write your own notes nest to the link of the page.

```
javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=  — notes to ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+') [[notes]]#quick-capture','Roam','toolbar=no,width=700,height=350'));
```
<a href="javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=  — notes to ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+') [[notes]]#quick-capture','Roam','toolbar=no,width=700,height=350'));">Comment to Roam</a>

Or just to open Quick Capture without text.

```
javascript:open('https://roamresearch.com/?text= #quick-capture','Roam','toolbar=no,width=700,height=350');
```
<a href="javascript:open%28%27https%3A%2F%2Froamresearch.com%2F%3Ftext%3D+%23quick-capture%27%2C%27Roam%27%2C%27toolbar%3Dno%2Cwidth%3D700%2Cheight%3D350%27%29%3B">Note to Roam</a>


## How to use

The bookmarklet uses the Mobile Quick Capture url integration (https://roamresearch.com/#/app/help/page/07-02-2020).

No need for copy-paste.

1. You can highlight a line of paragraph on a webpage and click the bookmarklet. 
2. A window popup will show you the same UI as on a mobile. You can add as many highlights or bookmarks as you want. 
3. To sync and see the captured text and url in Roam, you have to reload your app. A message asking if you want to sync the captured text will show.

This bookmarlet is adapted from the Pinboard bookmarklet. The text format is based on [+Roam](https://chrome.google.com/webstore/detail/%20roam/ekdmipoabmcjmlonhcdoijilfdoomjbm)

A better version of this page https://adolforismos.github.io/roam-quick-capture-bookmarklet/

By: [adolforismos](https://medium.com/@adolforismos)
