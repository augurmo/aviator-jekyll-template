---
title: projects
position: 1.1
type: post
description: Create Book
right_code: >-
  ~~~ json{  "id": 3,  "title": "The Book Thief",  "score": 4.3,  "dateAdded":
  "5/1/2015"}~~~{: title="Response" }~~~ json{  "error": true,  "message":
  "Invalid score"}~~~{: title="Error" }
---


<dl><dt>title</dt><dd>The title for the book [update by mo]</dd><dt>score</dt><dd>The book's score between 0 and 5</dd></dl>

The book will automatically be added to your reading list
{: .success}

Adds a book to your collection.

```javascript
$.post("http://api.myapp.com/books/", {
  "token": "YOUR_APP_KEY",
  "title": "The Book Thief [update by mo]",
  "score": 4.3
}, function(data) {
  alert(data);
});
```