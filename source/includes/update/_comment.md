## Update a comment ##

This API lets you make changes to a specific comment by ID.

```javascript
var data = {
  "content": "This comment has been removed by a moderator.",
};

restjQuery({
  endpoint: "comments/1",
  formMethod: "POST",
  postData: data
});
```
> Example updating a comments content should a moderator needed to.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-post">POST</i>
    <h6>/wp-json/wp/v2/comments/1</h6>
  </div>
</div>
