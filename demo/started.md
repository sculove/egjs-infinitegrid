### Browser support
IE 10+, latest of Chrome/FF/Safari, iOS 7+ and Android 2.3+ (except 3.x)

### Quick steps to use:


#### Set up your HTML

``` html
<!-- Target DOM -->
<ul id="grid">
    <li class="card">
        <div>test1</div>
    </li>
    <li class="card">
        <div>test2</div>
    </li>
    <li class="card">
        <div>test3</div>
    </li>
    <li class="card">
        <div>test4</div>
    </li>
    <li class="card">
        <div>test5</div>
    </li>
    <li class="card">
        <div>test6</div>
    </li>
</ul>
```

#### Load files or import library


##### ES5
``` html
{% for dist in site.data.egjs.dist %}
<script src="//{{ site.data.egjs.github.user }}.github.io/{{ site.data.egjs.github.repo }}/{{ dist }}"></script>
{% endfor %}
```


##### ES6+
```js
import InfiniteGrid from "@egjs/infinitegrid";
```

### Initialize it and all done!

#### ES5
```javascript
// create InfiniteGrid ui without option
new eg.InfiniteGrid("#grid");

// create InfiniteGrid ui with options
new eg.InfiniteGrid("#grid",{
  itemSelector: ".item"
});
```

#### ES6+
```javascript
// create InfiniteGrid ui without option
new InfiniteGrid("#grid");

// create InfiniteGrid ui with options
new InfiniteGrid("#grid",{
  itemSelector: ".item"
});
```