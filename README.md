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
new Cute.ui.dialog().alert('Hello', options || {});

// Notice
new Cute.ui.dialog().notice('Hello', options || {});

// Confirm
new Cute.ui.dialog().confirm('Are you sure you want to delete this item?', options || {});

// Loading
new Cute.ui.dialog().loading('Loading Text...', options || {});

// Ajax
new Cute.ui.dialog().ajax('Dialog Title', {
  action: 'xxx/get',  // api url
  params: {}, // querystring
  ajaxoptions: {} // ajax options
});

// Layer
new Cute.ui.dialog().layer('Dialog Title', {
  content: '#template'
});

// Iframe
new Cute.ui.dialog().iframe('Dialog Title', {
  url: 'xxx/xxx.html' // iframe src
});

// Tooltip
new Cute.ui.dialog().tooltip('layer', 'Tooltips', options || {});

// Suggest
new Cute.ui.dialog().suggest('Suggest text', options || {});

// Growl
new Cute.ui.dialog().growl('Growl text', options || {});
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
