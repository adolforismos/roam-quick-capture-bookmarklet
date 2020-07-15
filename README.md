# Roam Research quick capture bookmarklet
A simple bookmarklet to capture text from a webpage to Roam Research.

```
javascript:q=location.href;if(document.getSelection){d=document.getSelection();}else{d='';};p=document.title;void(open('https://roamresearch.com?text=__'+encodeURIComponent(d)+'__ — via ['+encodeURIComponent(p)+']('+encodeURIComponent(q)+')#quick-capture','Roam','toolbar=no,width=700,height=350'));
```
