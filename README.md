[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/grumpypufferfish/window-size)


## &lt;window-size&gt;

The `window-size` element manages data binding to the window&#39;s size. This component will most likely be used with other polymer components. If you are new to Polymer, the [Polymer website](https://www.polymer-project.org/) is the best place to start.

#### Properties

`window-size`'s properties are:

* `width`: window's width (window.innerWidth)
* `height`: window's height (window.innerHeight)

Since in most cases you can't change the size of a window in a browser via javascript (more info [here](https://developer.mozilla.org/en-US/docs/Web/API/Window/resizeTo)), the data bindings are unidirectional, i.e. flow upward (target to host) only.

`window-size` is only active while it is attached to the document.

#### Usage

`window-size` will more likely be used inside your Polymer element's template. In order to allow data binding to work outside a Polymer element, you need to wrap your code inside an auto-binding template, as shown in the following code snippet (new Polymer 2.0 syntax):

```html
<dom-bind>
  <template>
    <window-size width="{{width}}" height="{{height}}"></window-size>
    <div>
      <span>Width: {{width}} px</span>
      <span>Height: {{height}} px</span>
    </div>
  </template>
</dom-bind>
```

#### Notes

This component is based on the new Polymer 2.0 Release Candidate. Whilst waiting for a "stable release" of Polymer 2, this component is a pre-release.

