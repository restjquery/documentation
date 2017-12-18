# Posts #

The posts API allows you to create, view, update, and delete individual, or a batch, of posts.

## Post attributes ##

Attribute | Type | Description
--------- | ------- | -----------
`id` | integer | Unique identifier for the object.
`date` | string | The date the object was published, in the site's timezone.
`date_gmt` | string or datetime | The date the object was published, as GMT.
`slug` | string | An alphanumeric identifier for the object unique to its type.
`status` | string | A named status for the object. One of: `publish`, `future`, `draft`, `pending`, `private`
`password` | string | A password to protect access to the content and excerpt.
`title` | string | The title for the object.
`content` | string | The content for the object.
`author` | integer | The ID for the author of the object.
`excerpt` | string | The excerpt for the object.
`featured_media` | integer | The ID of the featured media for the object.
`comment_status` | string | Whether or not comments are open on the object. One of: open, closed
`ping_status` | string | Whether or not the object can be pinged. One of: open, closed
`format` | string | The format for the object. One of: standard, aside, chat, gallery, link, image, quote, status, video, audio
`meta` | object | Meta fields.
`sticky` | boolean | Whether or not the object should be treated as sticky.
`template` | string | The theme file to use to display the object.
`categories` | array | The terms assigned to the object in the category taxonomy.
`tags` | array | The terms assigned to the object in the post_tag taxonomy.
