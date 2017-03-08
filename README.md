# scalable
Scaling images based on ratio of container

### Options


#### container
Type: `object`

Default: window

#### items
Type: `function`

Default:

```js
  items: function(el, item, width, height, options) {
    $(el).find('ul li:eq('+ item +')>' + options.selector).css({ 'width': width + 'px', 'height': height +'px' })
  }
```

#### selector
Type: `string`

Default: 'span>img'

#### dimention
Type: Array

Default: `[]`

### Usage examples

```html
<div class="list-images">
  <ul>
    <li><span><img src="https://template-c.oncourse.cc/s/img/slides/slide-3.jpg"></span></li>
    <li><span><img src="https://template-c.oncourse.cc/s/img/slides/slide-1.jpg"></span></li>
  </ul>
</div>
```

```js
  $('.list-images').Scalable();
```
