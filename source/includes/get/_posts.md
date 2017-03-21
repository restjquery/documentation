# Posts #

## Get Posts ##

```javascript
var posts = restjQuery();
```

> JSON response example:

```json
[
  {
    "id":1,
    "date":"2017-01-04T15:46:25",
    "date_gmt":"2017-01-04T15:46:25",
    "guid":{
      "rendered":"http:\/\/experiments.dev\/?p=1"
    },
    "modified":"2017-01-04T15:46:25",
    "modified_gmt":"2017-01-04T15:46:25",
    "slug":"hello-world",
    "status":"publish",
    "type":"post",
    "link":"https:\/\/experiments.dev\/hello-world\/",
    "title":{
      "rendered":"Hello world!"
    },
    "content":{
      "rendered":"<p>Welcome to WordPress. This is your first post. Edit or delete it, then start writing!<\/p>\n",
      "protected":false
    },
    "excerpt":{
      "rendered":"<p>Welcome to WordPress. This is your first post. Edit or delete it, then start writing!<\/p>\n",
      "protected":false
    },
    "author":1,
    "featured_media":0,
    "comment_status":"open",
    "ping_status":"open",
    "sticky":false,
    "template":"",
    "format":"standard",
    "meta":[],
    "categories":[1],
    "tags":[],
    "_links":{
      "self":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/posts\/1"
        }
      ],
      "collection":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/posts"
        }
      ],
      "about":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/types\/post"
        }
      ],
      "author":[
        {
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/users\/1"
        }
      ],
      "replies":[
        {
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/comments?post=1"
        }
      ],
      "version-history":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/posts\/1\/revisions"
        }
      ],
      "wp:attachment":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/media?parent=1"
        }
      ],
      "wp:term":[
        {
          "taxonomy":"category",
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/categories?post=1"
        },
        {
          "taxonomy":"post_tag",
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/tags?post=1"
        }
      ],
      "curies":[
        {
          "name":"wp",
          "href":"https:\/\/api.w.org\/{rel}",
          "templated":true
        }
      ]
    }
  }
]
```

This lets you retrieve posts.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/posts</h6>
  </div>
</div>

## Get a Single Post ##

```javascript
var hello_world = restjQuery(
  endpoint: "posts/1"
);
```

> JSON response example:

```json
  {
    "id":1,
    "date":"2017-01-04T15:46:25",
    "date_gmt":"2017-01-04T15:46:25",
    "guid":{
      "rendered":"http:\/\/experiments.dev\/?p=1"
    },
    "modified":"2017-01-04T15:46:25",
    "modified_gmt":"2017-01-04T15:46:25",
    "slug":"hello-world",
    "status":"publish",
    "type":"post",
    "link":"https:\/\/experiments.dev\/hello-world\/",
    "title":{
      "rendered":"Hello world!"
    },
    "content":{
      "rendered":"<p>Welcome to WordPress. This is your first post. Edit or delete it, then start writing!<\/p>\n",
      "protected":false
    },
    "excerpt":{
      "rendered":"<p>Welcome to WordPress. This is your first post. Edit or delete it, then start writing!<\/p>\n",
      "protected":false
    },
    "author":1,
    "featured_media":0,
    "comment_status":"open",
    "ping_status":"open",
    "sticky":false,
    "template":"",
    "format":"standard",
    "meta":[],
    "categories":[1],
    "tags":[],
    "_links":{
      "self":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/posts\/1"
        }
      ],
      "collection":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/posts"
        }
      ],
      "about":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/types\/post"
        }
      ],
      "author":[
        {
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/users\/1"
        }
      ],
      "replies":[
        {
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/comments?post=1"
        }
      ],
      "version-history":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/posts\/1\/revisions"
        }
      ],
      "wp:attachment":[
        {
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/media?parent=1"
        }
      ],
      "wp:term":[
        {
          "taxonomy":"category",
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/categories?post=1"
        },
        {
          "taxonomy":"post_tag",
          "embeddable":true,
          "href":"https:\/\/experiments.dev\/wp-json\/wp\/v2\/tags?post=1"
        }
      ],
      "curies":[
        {
          "name":"wp",
          "href":"https:\/\/api.w.org\/{rel}",
          "templated":true
        }
      ]
    }
  }
```

This lets you retrieve and view a specific post.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/posts/1</h6>
  </div>
</div>
