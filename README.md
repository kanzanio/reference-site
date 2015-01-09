# Kanzan reference site

A simple reference site for a Kanzan site. This includes examples of each content type that you can manage in a site with Kanzan via http://kanzan.io


## Declaring Kanzan content

Kanzan understands HTML5 data attributes and will look for attributes that start with `data-kanzan-`. All attributes are optional except for `data-kanzan-id` and `data-kanzan-type`


## Kanzan attributes

- `data-kanzan-id` - A unique identifier for this field in the file.
- `data-kanzan-type` - The content type for this field.
- `data-kanzan-help` - Optional descriptive help text to display in the content admin site.
- `data-kanzan-label` - Optional label to display in the content admin site (`data-kanzan-id` used if not defined)


## Content types

### text

Defined by `data-kanzan-type="text"`

A simple short plain text field. This will create a text input field in the the content admin site.


### blob

Defined by `data-kanzan-type="blob"`

A longer plain text field. This will create a text area input field in the the content admin site.


### markdown

Defined by `data-kanzan-type="markdown"`

A longer text field which interprets markdown. This will create a text area input field in the the content admin site.
