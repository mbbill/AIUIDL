## Goal

This experimental project aims to improve the creation of AI-generated user interfaces. Currently, most UI language is designed for humans and can be challenging for AI to generate accurately or comprehend changes. The objective is to develop a method where users can request an AI-built interface with minimal unexpected outcomes during the process. Additionally, this approach will simplify rendering by allowing generated code to be easily displayed on-screen.

## Example:
Hi, this is the AIUIDL (AI User Interface Description Language) specification. [copy-paste the spec contents]
Please follow the specifications provided and generate the output for my user interface as described below:

The screen contains a central element that is 100x100 in size. This element consists of two buttons, each taking up half of the element's size. The button on the left should be green, while the button on the right should be blue.

## Output:
```json
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
```