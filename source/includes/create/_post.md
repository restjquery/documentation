## Create a post ##

This API helps you to create a new post.

```javascript
var data = {
  "title": "Hello World",
  "excerpt": "A \"Hello, World!\" program is a computer program that outputs or displays \"Hello, World!\" to a user. Being a very simple program in most programming languages, it is often used to illustrate the basic syntax of a programming language for a working program.[1] It is often the very first program people write when they are new to a language.",
  "content": "The phrase is also used by computer hackers as a proof of concept that arbitrary code can be executed through an exploit where the system designers did not intend code to be executed.",
  "status": "publish",
  "author": "1"
};

restjQuery({
  formMethod: "POST",
  postData: data
});
```

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-post">POST</i>
    <h6>/wp-json/wp/v2/posts</h6>
  </div>
</div>
