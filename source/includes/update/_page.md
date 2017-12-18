## Update a page ##

This API lets you make changes to a specific page by ID.

```javascript
var data = {
  "title": "Contribute to WP REST API jQuery",
};

restjQuery({
  endpoint: "pages/2",
  formMethod: "POST",
  postData: data
});
```
> Example updating "Contribute to REST jQuery" post title.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-post">POST</i>
    <h6>/wp-json/wp/v2/pages/2</h6>
  </div>
</div>
