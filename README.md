# vue-js-spatial-navigation [![npm version](http://img.shields.io/npm/v/vue-js-spatial-navigation.svg?style=flat)](https://npmjs.org/package/vue-js-spatial-navigation "View this project on npm")

Forked from [spacerefugee](https://github.com/spacerefugee/vue-js-spatial-navigation)

### Updated to be compatible with Vue3

- Added mouse support
- Added click event trigger key-up on focused element
- Added directive 'v-focus-events' for spatial navigation custom events

Vue directive of [js-spatial-navigation](https://github.com/luke-chang/js-spatial-navigation);

## Installation

### NPM

```shell
    npm install vue-js-spatial-navigation
```

## Getting Started

```javascript
import Vue from "vue";
import vjsn from "vue-js-spatial-navigation";

Vue.use(vjsn);
```

#### Optional global [Configuration](https://github.com/luke-chang/js-spatial-navigation#configuration)

#### Additional configuration `scrollOptions`:

- The page will auto scroll to the focus element by using [`scrollIntoView`](https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollIntoView).

- You can set this `scrollOptions` for the `scrollIntoViewOptions`.

- The page will not scroll to the focus element when setting `scrollOptions` to `""` or `null`.

```javascript
const config = {
  straightOnly: false,
  straightOverlapThreshold: 0.5,
  rememberSource: false,
  disabled: false,
  defaultElement: "",
  enterTo: "",
  leaveFor: null,
  restrict: "self-first",
  tabIndexIgnoreList:
    "a, input, select, textarea, button, iframe, [contentEditable=true]",
  navigableFilter: null,
  scrollOptions: { behavior: "smooth", block: "center" },
};
Vue.use(vjsn, config);
```

## Documentation

### `$SpatialNavigation`

A global Vue instance property for [SpatialNavigation](https://github.com/luke-chang/js-spatial-navigation#api-reference);

```javascript
// you can access SpatialNavigation in every instance
this.$SpatialNavigation;
```

### [`v-focus`](https://github.com/Syncronet-APS/vue-js-spatial-navigation/blob/master/docs/v-focus.md)

### [`v-focus-events`](https://github.com/Syncronet-APS/vue-js-spatial-navigation/blob/master/docs/v-focus-events.md)

### [`v-focus-section`](<(https://github.com/Syncronet-APS/vue-js-spatial-navigation/blob/master/docs/v-focus-section.md)>)

### [`v-disable-focus-section`](<(https://github.com/Syncronet-APS/vue-js-spatial-navigation/blob/master/docs/v-disable-focus-section.md)>)
