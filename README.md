# Vuex Composition API demo

## Deployment

- Checkout deployment at https://gagandeep39.github.io/vuex-composition-api-demo/

## Other composition API projects

- Basic demo https://github.com/Gagandeep39/vue-composition-api-demo
- Project Viewver (Advanced) https://github.com/Gagandeep39/project-viewer-vue
- Project Management with Routing https://github.com/Gagandeep39/product-management-system-vue

## Store in Compoistion API

```js
import { useStore } from 'vuex';

export default {
  setup() {
    const store = useStore();
    // Dispatching
    function inc() {
      store.dispatch('increment');
    }
    // Fetching data
    const counter = computed(() => store.getters.counter);
    return { inc };
  },
};
```
