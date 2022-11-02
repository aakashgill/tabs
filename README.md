# Auto tabs
---

A simple tabs switcher with an autoplay feature
1. Support for multiple instances of tabs
2. Support of setting the autoplay timer


## Get started by adding the
### Markup
``` HTML
<div id="tabs">
    <div class="tabs-container">
        <button data-tab="tab1" class="tabs active-tab">
            Tab 1
        </button>
        <button data-tab="tab2" class="tabs">
            Tab 2
        </button>
        <button data-tab="tab3" class="tabs">
            Tab 3
        </button>
        <button data-tab="tab4" class="tabs">
            Tab 4
        </button>
    </div>
    <div class="tabs-content-container">
        <div class="tab-content active-tab" data-tab-content="tab1">
            Tab 1 data
        </div>
        <div class="tab-content" data-tab-content="tab2">
            Tab 2 data
        </div>
        <div class="tab-content" data-tab-content="tab3">
            Tab 3 data
        </div>
        <div class="tab-content" data-tab-content="tab4">
            Tab 4 data
        </div>
    </div>
</div>
```

### CSS
``` CSS
.tabs-content-container .tab-content {
    display: none;
}
.tabs-content-container .tab-content.active-tab {
    display: block;
}
```

### JS
``` HTML
<script src="path_goes_here/auto-tabs.js"></script>
<script>
    new Tabs({
        el: '#tabs'
    });
</script>
```


## Options
| Name | Value | Default Value | Optional |
| --- | --- | --- | --- |
| autoplay | true/false | true | yes |
| timer | 1000 | 2000 | yes |


### For example
```JS
new Tabs({
    el: '#tabs',
    autoplay: false
});
```