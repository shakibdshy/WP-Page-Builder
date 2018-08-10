# BoxShadow 
A Box-shadow input field

## Parameters
Parameter | Type | Value
--- | --- | ---
type | `required` | Predefined String (textarea)
title | `optional` | String
desc | `optional` | String
std | `optional` | Array

## Return
Always return `object`

## Example
```php
'widget_boxshadow' => array(
	'type' => 'boxshadow',
	'title' => 'Boxshadow Field',
	'std' => array(
		    'shadowValue'=> array( 'top' => '120px', 'right' => '0px', 'bottom' => '0px', 'left' => '0px' ), 
		    'shadowColor' 	=> '#ffffff' 
			),
	'selector' => '{{SELECTOR}} .example-boxshadow'
)
```
Support 'selector' parameters.


## Controls
### PHP
Inside the `rander()` method-
```php
echo '<div>'.$data["settings"]["widget_boxshadow"]["shadowValue"]["top"].'</div>';
echo '<div>'.$data["settings"]["widget_boxshadow"]["shadowColor"].'</div>';
```

### JS Template
Inside the `getTemplate()` method-
```js
<div>{{data.widget_border.shadowValue.top}}</div>
<div>{{data.widget_border.shadowColor}}</div>
```