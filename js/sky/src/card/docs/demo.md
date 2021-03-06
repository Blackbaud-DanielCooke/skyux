---
name: Card
icon: th-large
summary: The card component creates a small container to highlight important information.
---

The card directive creates a small container to highlight important information. Generally, multiple cards are organized together to display information about a collection of related items. For example, cards can present a stack or carousel of to-do items or a matrix of images.

Cards frequently present users with a call to action. They can use visual cues to alert users about the need for action, and they can also include actions directly on the cards.

You can modify cards to handle a variety of scenarios, but they generally consist of three main parts: a title to identify what the card represents, content to display in the body of the card, and an action to let users act on the card. Each item is optional.

### Card settings ###
- `bb-card` &mdash; Creates a small container to highlight important information.
    - `bb-card-selection-toggled` &mdash; *(Optional.)* Specifies a callback that will be executed when a user toggles the card selection. It has the following arguments: 
      - `isSelected` &mdash; Set to true if the card is selected, set to false otherwise.
    - `bb-card-size` &mdash; *(Optional.)* Specifies the size of the card. For a large container, specify `large`. For a small container, specify `small`. *(Default: `large`)*
    - `bb-card-selectable` &mdash; *(Optional.)* Specifies whether to display a checkbox to the right of the title. Users can select the checkbox for one or more cards to then perform an action on the selected cards.
    - `bb-card-selected` &mdash; *(Optional.)* Specifies whether the card is selected (i.e. its checkbox is checked). When the user selects the card the specified property on your model will be updated accordingly.
    - `bb-card-title` &mdash; Specifies a title to identify the content that the card displays. The title is not required, but we recommend that you include it except in special circumstances. For example, you might exclude the title if a card displays an image with a filename that won't convey anything to users and the image itself is the most important content.
    - `bb-card-content` &mdash; Specifies the content to display in the body of the card. The type of content depends on what the card represents and whether it prompts users to action. Content can consist of some combination of a graph, trend, status, summary information, and guidance text.
    - `bb-card-actions` &mdash; Specifies an action or multiple actions for users to act on the intent of the card. To display a single action, use a `button` element within `bb-card-actions`. To display multiple actions, use [the `bb-context-menu` directive](../contextmenu) within `bb-card-actions`.
