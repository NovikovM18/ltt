<template>
  <div>
    <ReqComp 
      :item="item" 
      :index="index"
      v-for="(item, index) in arr" 
      :key="item.id"
      @click="clearSelected"
    />
  </div>
</template>
<script>
import ReqComp from '@/components/ReqComp';
export default {
  components: {
    ReqComp
  },
  data() {
    return {
      arr: [
  {
    id: 1,
    name: '1',
    children: [
      {
        id: 11,
        name: '11',
        children: [
          {
            id: 111,
            name: '111',
            children: [
              {
                id: 1111,
                name: '1111',
                children: []
              },
              {
                id: 11111,
                name: '11111',
                children: []
              },
            ]
          },
          {
            id: 111,
            name: '111',
            children: [
              {
                id: 1111,
                name: '1111',
                children: [
                  {
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: []
                      },
                    ]
                  },
                  {
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: []
                      },
                    ]
                  },
                ]
              },
              {
                id: 11111,
                name: '11111',
                children: [
                  {
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: [
                          {
                            id: 111,
                            name: '111',
                            children: [
                              {
                                id: 1111,
                                name: '1111',
                                children: []
                              },
                              {
                                id: 11111,
                                name: '11111',
                                children: []
                              },
                            ]
                          },
                        ]
                      },
                    ]
                  },
                ]
              },
            ]
          },
        ]
      },
    ]
  },
  {
    id: 2,
    name: '2',
    children: [
      {
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: []
          },
          {
            id: 11111,
            name: '11111',
            children: []
          },
        ]
      },{
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: []
          },
          {
            id: 11111,
            name: '11111',
            children: []
          },
        ]
      },{
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: [{
              id: 111,
              name: '111',
              children: [
                {
                  id: 1111,
                  name: '1111',
                  children: [{
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: [{
                          id: 111,
                          name: '111',
                          children: [
                            {
                              id: 1111,
                              name: '1111',
                              children: [{
                                id: 111,
                                name: '111',
                                children: [
                                  {
                                    id: 1111,
                                    name: '1111',
                                    children: []
                                  },
                                  {
                                    id: 11111,
                                    name: '11111',
                                    children: [{
                                      id: 111,
                                      name: '111',
                                      children: [
                                        {
                                          id: 1111,
                                          name: '1111',
                                          children: []
                                        },
                                        {
                                          id: 11111,
                                          name: '11111',
                                          children: [{
                                            id: 111,
                                            name: '111',
                                            children: [
                                              {
                                                id: 1111,
                                                name: '1111',
                                                children: []
                                              },
                                              {
                                                id: 11111,
                                                name: '11111',
                                                children: []
                                              },
                                            ]
                                          },]
                                        },
                                      ]
                                    },]
                                  },
                                ]
                              },]
                            },
                            {
                              id: 11111,
                              name: '11111',
                              children: []
                            },
                          ]
                        },]
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: []
                      },
                    ]
                  },]
                },
                {
                  id: 11111,
                  name: '11111',
                  children: []
                },
              ]
            },]
          },
          {
            id: 11111,
            name: '11111',
            children: []
          },
        ]
      },
    ]
  },
  {
    id: 3,
    name: '3',
    children: [
      {
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: []
          },
          {
            id: 11111,
            name: '11111',
            children: [{
              id: 111,
              name: '111',
              children: [
                {
                  id: 1111,
                  name: '1111',
                  children: []
                },
                {
                  id: 11111,
                  name: '11111',
                  children: [{
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: [{
                          id: 111,
                          name: '111',
                          children: [
                            {
                              id: 1111,
                              name: '1111',
                              children: []
                            },
                            {
                              id: 11111,
                              name: '11111',
                              children: []
                            },
                          ]
                        },]
                      },
                    ]
                  },]
                },
              ]
            },]
          },
        ]
      },
    ]
  },
  {
    id: 4,
    name: '4',
    children: [
      {
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: []
          },
          {
            id: 11111,
            name: '11111',
            children: []
          },
        ]
      },
    ]
  },
  {
    id: 5,
    name: '5',
    children: [
      {
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: [{
              id: 111,
              name: '111',
              children: [
                {
                  id: 1111,
                  name: '1111',
                  children: []
                },
                {
                  id: 11111,
                  name: '11111',
                  children: [{
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: []
                      },
                    ]
                  },]
                },
              ]
            },]
          },
          {
            id: 11111,
            name: '11111',
            children: [{
              id: 111,
              name: '111',
              children: [
                {
                  id: 1111,
                  name: '1111',
                  children: []
                },
                {
                  id: 11111,
                  name: '11111',
                  children: []
                },
              ]
            },]
          },
        ]
      },
    ]
  },
  {
    id: 6,
    name: '6',
    children: [
      {
        id: 111,
        name: '111',
        children: [
          {
            id: 1111,
            name: '1111',
            children: [{
              id: 111,
              name: '111',
              children: [
                {
                  id: 1111,
                  name: '1111',
                  children: [{
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: []
                      },
                    ]
                  },]
                },
                {
                  id: 11111,
                  name: '11111',
                  children: [{
                    id: 111,
                    name: '111',
                    children: [
                      {
                        id: 1111,
                        name: '1111',
                        children: []
                      },
                      {
                        id: 11111,
                        name: '11111',
                        children: []
                      },
                    ]
                  },]
                },
              ]
            },]
          },
          {
            id: 11111,
            name: '11111',
            children: [{
              id: 111,
              name: '111',
              children: [
                {
                  id: 1111,
                  name: '1111',
                  children: []
                },
                {
                  id: 11111,
                  name: '11111',
                  children: []
                },
              ]
            },]
          },
        ]
      },
    ]
  },
]
    }
  },
  mounted() {
    this.deSelected(this.arr);
  },
  methods: {
    deSelected(arr) {
      for(let i = 0; i < arr.length; i++) {
        arr[i].selected = false;
        if(arr[i].children.length > 0) {
          this.deSelected(arr[i].children);
        }
      }
    },
    clearSelected() {
      this.deSelected(this.arr);
    }

  }
}
</script>

<style lang="scss">

</style>
