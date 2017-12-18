## Update a post ##

This API lets you make changes to a specific post by ID.

```javascript
var data = {
  "title": "Kitty",
};

restjQuery({
  endpoint: "posts/1",
  formMethod: "POST",
  postData: data
});
```
> Example updating "Hello World" post title.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-post">POST</i>
    <h6>/wp-json/wp/v2/posts/1</h6>
  </div>
</div>
