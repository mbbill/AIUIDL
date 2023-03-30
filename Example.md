Prompt:
Hi, this is the AIUIDL (AI User Interface Description Language) specification. [spec contents]
Please follow the specifications provided and generate the output for my user interface as described below:

The screen contains a central element that is 100x100 in size. This element consists of two buttons, each taking up half of the element's size. The button on the left should be green, while the button on the right should be blue.

Output:
{
  "id": "root",
  "type": "container",
  "style": {
    "width": "100%",
    "height": "100%",
    "display": "flex",
    "justifyContent": "center",
    "alignItems": "center"
  },
  "children": [
    {
      "id": "element",
      "type": "container",
      "style": {
        "width": "100px",
        "height": "100px",
        "display": "flex"
      },
      "children": [
        {
          "id": "leftButton",
          "type": "button",
          "style": {
            "width": "50%",
            "height": "100%",
            "backgroundColor": "green"
          },
          "children": [
            {
              "id": "leftButtonText",
              "type": "text",
              "content": "Left Button"
            }
          ]
        },
        {
          "id": "rightButton",
          "type": "button",
          "style": {
            "width": "50%",
            "height": "100%",
            "backgroundColor": "blue"
          },
          "children": [
            {
              "id": "rightButtonText",
              "type": "text",
              "content": "Right Button"
            }
          ]
        }
      ]
    }
  ]
}
