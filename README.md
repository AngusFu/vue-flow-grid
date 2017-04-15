# v-flow

A simple waterfall directive for Vue.js.

## How to use

### Install

`npm install --save v-flow`

or

`yarn add v-flow`

### Import

```js
    import Vue from 'vue';
    import VFlow from 'v-flow';
    Vue.use(VFlow);
```

### Example

```html
<ul v-flow="3">
    <li>Lorem ipsum dolor sit amet.</li>
    <li>Eum at possimus eos soluta.</li>
    <li>Veniam quidem, repudiandae blanditiis vitae.</li>
    <li>Et ratione, nobis placeat corporis.</li>
    <li>Facere dolore, tenetur incidunt facilis.</li>
    <li>Quis obcaecati a qui iusto.</li>
    <li>Necessitatibus, illum odit eius cum?</li>
    <li>Vel nisi vero eos velit?</li>
</ul>
```

The code above will be transformed to:

```html
<ul>
    <div style="width: 33.3333%; float: left;">
        <li style="visibility: visible;">Lorem ipsum dolor sit amet.</li>
        <li style="visibility: visible;">Et ratione, nobis placeat corporis.</li>
        <li style="visibility: visible;">Necessitatibus, illum odit eius cum?</li>
    </div>
    <div style="width: 33.3333%; float: left;">
        <li style="visibility: visible;">Veniam quidem, repudiandae blanditiis vitae.</li>
        <li style="visibility: visible;">Facere dolore, tenetur incidunt facilis.</li>
        <li style="visibility: visible;">Vel nisi vero eos velit?</li>
    </div>
    <div style="width: 33.3333%; float: left;">
        <li style="visibility: visible;">Eum at possimus eos soluta.</li>
        <li style="visibility: visible;">Quis obcaecati a qui iusto.</li>
    </div>
    <i style="clear: both;"></i>
</ul>
```

### TODO LIST

- test cases
