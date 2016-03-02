# WordPress Tags-Like Meta Box

The WordPress tags meta box has a great interface for dealing with data. 
This helper class will allow you to customize a tags-like meta box of your own with ease.


##Use

Include the class file anywhere (in your plugin or theme), and then instantiate the class.

```php
$myVersionOfTags = new Tags_Like_Meta_box( 
    array( 
        'ID' => 'post-notes', 
        'nice_name' => 'Notes',
        'screen' => 'page',
		'howto' => 'Separate data with commas'
    )
);
```

`ID` specifies the name custom field name for your data.  
`nice_name` is the name which is displayed to the user.  
`screen`, `context` and `priority` can be used with the parameters described in the [add_meta_box()](https://developer.wordpress.org/reference/functions/add_meta_box/)-reference.  
`howto` adds an explanation.
`nojstext` adds an explanation if there's no javascript.
