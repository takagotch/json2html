### json2html
---
http://json2html.com/

```js
var transform = {
  "list":{"<>":"ul","html":function(){
  
  }},
  
  "items":{"<>":"li","html":function(){
    return( (index+1) + ". " + obj.title);
  }, "onclick":function(e){
    $("#example-jquery-app-output .details").empty().json2html(e.obj,transform.details);
  }},
  
  "details":[
    {"<>":"div","html":[
      {"<>":"h5","text":"${title}"}
    ]},
    {"<>":"div","text":"Year: ${year}"},
    {"<>":"div","text":"Rating: ${rating}"},
  ]
};

var data = [
  {"title":"The Shawshank Redemption","year":"1994","rating":"9.2"},
  {"title":"The Godfather","year":"1972","rating":"9.2"},
  {"title":"The Godfather: Part II","year":"1974","rating":"9.0"},
  {"title":"The Dark Knight","year":"2008","rating":"9.0"},
  {"title":"12 Angry Men","year":"1957","rating":"9.0"},
];

$("#example-jquery-app-output .list").json2html({},transforms.list);
```

```
```

```
```


