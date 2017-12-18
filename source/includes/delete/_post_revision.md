## Delete a post revision ##

This API lets you delete a specific post revision by ID.

<aside class="notice">Replace <strong>parent_ID</strong> with the post ID the post revision is associated with. Replace <strong>revision_ID</strong> with the revision ID you want to delete.</aside>

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-delete">DELETE</i>
    <h6>/wp-json/wp/v2/posts/1/revisions/43</h6>
  </div>
</div>

```javascript
restjQuery({
  endpoint: "posts/<parent_ID>/revisions/<revision_ID>",
  formMethod: "DELETE",
});
```
