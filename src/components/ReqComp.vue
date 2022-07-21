<template>
  <div>
    <p 
      @click="showParent(item)"
      v-bind:class="item.selected ? 'selected' : ''"
    >
      {{ item.name }} + {{ item.name }}
    </p>
    <div>
      <div>
        <ul v-if="item.children && item.children.length > 0">
          <ReqComp 
            v-for="(child, subIndex) in item.children" 
            v-bind:item="child"
            :index="subIndex"
            :key="child.id"
            :parentItem="item"
            @showParent="showParent"
            />
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "ReqComp",
  props: {
    item: {
      type: Object,
      required: true
    },
    index: {
      type: Number,
      required: true
    },
    parentItem: {
      required: false
    }
  },
  methods: {
    showParent(item) {
      if (this.parentItem) {
        console.log('parent element: ' + this.parentItem.id + '+' + this.parentItem.name);
        }
      else {
        console.log('this element doesn`t have parent element');
      }
      setTimeout((() => item.selected = true), 0)
    },

  }
}
</script>

<style lang="scss" scoped>
p {
  cursor: pointer;
}
p:hover {
  background-color: deepskyblue;
}
.selected {
  background-color: dodgerblue;
}
</style>