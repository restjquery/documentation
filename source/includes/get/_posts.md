## List posts ##

This API helps you to list all the posts that have been created.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/posts</h6>
  </div>
</div>

#### Available parameters ####

Attribute | Type | Description
--------- | ------- | -----------
`page` | integer | Current page of the collection.
`per_page` | integer | Maximum number of items to be returned in result set.
`search` | string | Limit results to those matching a string.
`after` | date | Limit response to posts published after a given ISO8601 compliant date.
`author` | integer | Limit results set to posts assigned to specific authors.
`author_exclude` | integer | Ensure result set excludes posts assigned to specific authors.
`before` | date | Limit response to posts published before a given ISO8601 compliant date.
`exclude` | array | Ensure result set excludes specific IDs.
`include` | array | Ensure result set includes specific IDs.
`offset` | | Offset the result set by a specific number of items.
`order` | `asc` or `desc` | Order sort attribute ascending or descending.
`order_by` | `author`, `date`, `id`, `include`, `modified`, `parent`, `relevance`, `slug`, `title` | Sort collection by object attribute.
`slug` | string | Limit result set to posts with one or more specific slugs.
`status` | string | Limit result set to posts assigned one or more statuses. One of: `publish`, `future`, `draft`, `pending`, `private`
`categories` | array | Limit result set to all items that have the specified term assigned in the categories taxonomy.
`categories_exclude` | array | Limit result set to all items except those that have the specified term assigned in the categories taxonomy.
`tags` | array | Limit result set to all items that have the specified term assigned in the tags taxonomy.
`tags_exclude` | array | Limit result set to all items except those that have the specified term assigned in the tags taxonomy.
`sticky` | boolean | Limit result set to items that are sticky.

```javascript
var posts = restjQuery(
  endpoint: "posts"
);
```

> JSON response example:

```json
[
  {
    "id":1,
    "date":"2017-01-04T15:46:25",
    "date_gmt":"2017-01-04T15:46:25",
    "guid":{
      "rendered":"http:\/\/restjquery.dev\/?p=1"
    },
    "modified":"2017-01-04T15:46:25",
    "modified_gmt":"2017-01-04T15:46:25",
    "slug":"hello-world",
    "status":"publish",
    "type":"post",
    "link":"https:\/\/restjquery.dev\/hello-world\/",
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
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/posts\/1"
        }
      ],
      "collection":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/posts"
        }
      ],
      "about":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/types\/post"
        }
      ],
      "author":[
        {
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/users\/1"
        }
      ],
      "replies":[
        {
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/comments?post=1"
        }
      ],
      "version-history":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/posts\/1\/revisions"
        }
      ],
      "wp:attachment":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/media?parent=1"
        }
      ],
      "wp:term":[
        {
          "taxonomy":"category",
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/categories?post=1"
        },
        {
          "taxonomy":"post_tag",
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/tags?post=1"
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

## Retrieve a post ##

This API helps you to retrieve and view a specific post by ID.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/posts/1</h6>
  </div>
</div>

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
      "rendered":"http:\/\/restjquery.dev\/?p=1"
    },
    "modified":"2017-01-04T15:46:25",
    "modified_gmt":"2017-01-04T15:46:25",
    "slug":"hello-world",
    "status":"publish",
    "type":"post",
    "link":"https:\/\/restjquery.dev\/hello-world\/",
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
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/posts\/1"
        }
      ],
      "collection":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/posts"
        }
      ],
      "about":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/types\/post"
        }
      ],
      "author":[
        {
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/users\/1"
        }
      ],
      "replies":[
        {
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/comments?post=1"
        }
      ],
      "version-history":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/posts\/1\/revisions"
        }
      ],
      "wp:attachment":[
        {
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/media?parent=1"
        }
      ],
      "wp:term":[
        {
          "taxonomy":"category",
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/categories?post=1"
        },
        {
          "taxonomy":"post_tag",
          "embeddable":true,
          "href":"https:\/\/restjquery.dev\/wp-json\/wp\/v2\/tags?post=1"
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
