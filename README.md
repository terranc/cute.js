# Usage

## Ajax

```js
Cute.api.ajax(type, action, data, callback, cache, async, options)

// GET
Cute.api.get(action, data, callback, cache, async, options)

// POST
Cute.api.post(action, data, callback, cache, async, options)
```

## Dialog

```js
// Alert Modal
var dialog = new Cute.ui.dialog().alert('Hello', options || {});

// Notice
var dialog = new Cute.ui.dialog().notice('Hello', options || {});

// Confirm
var dialog = new Cute.ui.dialog().confirm('Are you sure you want to delete this item?', options || {});

// Loading
var dialog = new Cute.ui.dialog().loading('Loading Text...', options || {});

// Ajax
var dialog = new Cute.ui.dialog().ajax('Dialog Title', {
  action: 'xxx/get',  // api url
  params: {}, // querystring
  ajaxoptions: {} // ajax options
});

// Layer
var dialog = new Cute.ui.dialog().layer('Dialog Title', {
  content: '#template'
});

// Iframe
var dialog = new Cute.ui.dialog().iframe('Dialog Title', {
  url: 'xxx/xxx.html' // iframe src
});

// Tooltip
var dialog = new Cute.ui.dialog().tooltip('layer', 'Tooltips', options || {});

// Suggest
var dialog = new Cute.ui.dialog().suggest('Suggest text', options || {});

// Growl
var dialog = new Cute.ui.dialog().growl('Growl text', options || {});


// Methods
dialog.resize({
  width: xxx,  // optional
  height: xxx,  // optional
})


dialog.setClassName(name)

dialog.setButtons(buttions) // (array) buttons

dialog.setPos(pos)  // (object) pos: css position

dialog.setTitle(title)

dialog.setFoot(html, ?reset)  // reset: `true` is replace; `false` is append

dialog.setContent(html) // set inner content

dialog.setHtml(html)    // set wrap content

dialog.show()

dialog.hide()

dialog.close()

dialog.toggle();
```


## Pager

```js
new Cute.ui.pager('#pager', {
  pageindex: 0,
  pagesize: 10,
  totalcount: -1,
  pagecount: 0,
  currpagetotal: -1,  // if equal `-1` then hide page number selector
  type: "numeric", // `numeric` or `text`
  total: false, // show total number ?
  skip: false,  // show page input ?
  breakpage: 5,
  ajaxload: false,
  ajaxcallback: $.noop
})
```

## Select

```js
new Cute.ui.select('select[name=category_id]')
```
