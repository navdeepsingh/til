# Event handle on dynamic loaded element

Suppose we have dynamic loaded element with class test in html as follows

```html
<div id="container">
	<a href="" class="test">Dynamic Link</a>
</div>
```

```javascript

$('#container').on('click', 'a.test', function() {
	console.log('I am clicked');
});

```