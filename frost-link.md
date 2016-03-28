# ember-frost-link <br />
* [API](#api)
* [Examples](#examples)

## API

| Attribute | Type | Value | Description |
| --------- | ---- | ----- | ----------- 
| `priority` | `string` | `primary` | primary link - opens content in a new tab |
|  |  | `secondary` | secondary link - opens content in the same tab |
|  |  | `tertiary` | tertiary link - opens content in the same tab |
| `size` | `string` | `small` | small size link |
|  |  | `medium` | medium size link |
|  |  | `large` | large size link |
| `design` | `string` | `info-bar` | custom link styling for the info-bar context.  Requires `icon` to be specified.  Should not be used with `priority` and `size`. |
| `disabled` | `boolean` | `false` | **default** - basic link |
|  |  | `true` | disabled link |
| `icon` | `string` | `<icon-name>` | the name of a frost-icon |


## Examples

### Primary - small
```handlebars
{{#frost-link 'route name'
  priority='primary'
  size='small'
}}
  Primary
{{/frost-link}}
```

### Primary - medium
```handlebars
{{#frost-link 'route name'
  priority='primary'
  size='medium'
}}
  Primary
{{/frost-link}}
```

### Secondary - large
```handlebars
{{#frost-link 'route name'
  priority='secondary'
  size='large'
}}
  Secondary
{{/frost-link}}
```

### Tertiary - Size based on font
```handlebars
{{#frost-link 'route name'
  priority='tertiary'
}}
  Link one
{{/frost-link}}
```

### Primary - disabled
```handlebars
{{#frost-link 'route name'
  priority='primary'
  size='small'
  disabled=true
}}
  Primary
{{/frost-link}}
```

### Design - info-bar
```handlebars
{{#frost-link 'route name'
  design='info-bar'
  icon='icon'
}}
  Action
{{/frost-link}}
```