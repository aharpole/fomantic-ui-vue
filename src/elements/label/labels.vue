<template>
  <div :class="classes">
    <slot />
  </div>
</template>

<script>
import u from '../../lib/util';
// import Enum from '../../lib/enum';
import Mixins from '../../lib/mixins';

export default {
  name: 'FuiLabels',
  mixins: [
    Mixins.PColor,
  ],
  props: {
    basic: {
      type: Boolean,
      description: '', // TODO: descr
    },
    tagged: {
      type: Boolean,
      description: '', // TODO: descr
    },
    circular: {
      type: Boolean,
      description: '', // TODO: descr
    },
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
        this.basic && 'basic',
        this.circular && 'circular',
        this.tagged && 'tag',
        ...this.getClassesColor,
        'labels'
      );
    },
  },
};
</script>
