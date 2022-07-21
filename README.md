1. Setup VUE 3 app via vue cli. (no router needed)
2. You'll have an array with "unknown" depth of children included.
3. You should setup architecture to handle this array recursivelyб with the help of components and subcomponents and show id+name keys in UI. Every child array should have additional css indent. 
5. Every item should have a click event with the ability to toggle parameter: {selected: true} (if there is no key:value pair like this it should be added to the object) and should be highlighted in the list via css somehow(background, color, underline etc). When some element gets highlighted, other elements should get selected: false param. Basically only 1 highlighted element should be in the tree.
4.  to show (.log/alert) their parent element.

arr = [
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