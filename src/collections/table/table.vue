<template>
  <table :class="classes">
    <slot />
  </table>
</template>

<script>
import u from '../../lib/util';
// import Enum from '../../lib/enum';
// import Mixins from '../../lib/mixins';

export default {
  name: 'FuiTable',
  mixins: [],
  props: {
    definition: {
      type: Boolean,
      description: '', // TODO: descr
    },
    /*
    prop1: { // TODO: Component FuiTable
      type: Boolean,
      description: '',
    },
    prop2: {
      type: String,
      description: '',
      default: '',
    },
    prop3: {
      type: String,
      description: '',
      validator: (value) => {
        return !value || Enum.LeftRight.check(value);
      },
      default: '',
    },
    */
  },
  events: {
    click: {
      description: 'Click event',
    },
  },
  computed: {
    classes: function () {
      return u.concatClasses(
        'ui',
        this.definition && 'definition',
        'table'
      );
    },
  },
};
</script>
