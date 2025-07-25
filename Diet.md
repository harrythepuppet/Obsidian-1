{

  "replace": false,

  "groups": [

    "fruits",

    "grains",

    "proteins",

    "sugars",

    "vegetables"

  ],

  "effects": [

    {

      "attributes": [

        {

          "name": "minecraft:generic.max_health",

          "operation": "add",

          "amount": 1.0

        }

      ],

      "conditions": [

        {

          "groups": ["proteins", "fruits", "vegetables", "grains"],

          "match": "every",

          "above": 0.75,

          "below": 1.0

        }

      ]

    },

    {

      "attributes": [

        {

          "name": "minecraft:generic.movement_speed",

          "operation": "multiply_base",

          "amount": 0.8

        }

      ],

      "conditions": [

        {

          "groups": ["sugars"],

          "match": "all",

          "above": 0.75,

          "below": 1.0

        }

      ]

    }

  ]

}