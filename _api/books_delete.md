---
title: /books/:id
position: 1.5
type: get
description: Deletes a book中午中午zhongwen中午中午中文中午中午中文zho
right_code: |
  ~~~ json
  {
    "id": 3,
    "status": "deleted"
  }
  ~~~
  {: title="Response" }

  ~~~ json
  {
    "error": true,
    "message": "Book d中午中午中文中文hhoesn't exist"
  }
  ~~~
  {: title="Error" }
---
Deletes a book in your collection.

~~~ javascript
$.ajax({
  "url": "http://api.myapp.com/books/3",
  "type": "DELETE",
  "data": {
    "token": "YOUR_APP_KEY"
  },
  "success": function(data) {
    alert(data);
  }
});
~~~
{: title="jQuery" }
