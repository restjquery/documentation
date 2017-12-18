## Create a page ##

This API helps you to create a new page.

```javascript
var data = {
  "title": "Contribute to REST jQuery",
  "excerpt": "I am looking for contributors to help improve the authentication methods used to be more secure and provide a great first solution to supporting a callback method. If you are interested then please let me know.",
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
    <h6>/wp-json/wp/v2/pages</h6>
  </div>
</div>
