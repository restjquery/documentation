## List post revisions ##

This API helps you to list all the post revisions that have been created for a parent post ID.

<aside class="notice">Replace <strong>parent_ID</strong> with the post ID the post revisions are associated with.</aside>

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/posts/1/revisions</h6>
  </div>
</div>

```javascript
var post_revisions = restjQuery(
  endpoint: "posts/<parent_ID>/revisions"
);
```

> JSON response example:

```json
code response goes here
```
