# Vue Vertical Timeline
This is a simple vertical timeline component made with vueJs.
## Getting started
### npm

Use the package manager [npm](https://www.npmjs.com/package/) to install this.
```bash
npm install vue-vertical-timeline
```

### yarn
You can also use yarn.

```bash
yarn add vue-vertical-timeline
```

## Usage

Without any configuration, you can render the component with the default props.


```HTML
<vertical-timeline />
```

And then import and initialize the component:

```JavaScript
import Vue from 'vue'
import VerticalTimeline from 'vue-vertical-timeline'


Vue.use(VerticalTimeline);
```

## NuxtJs


You can import as a Nuxt.js plugin

`~/plugins/vue-vertical-timeline.js`

```js
import Vue from "vue";
import VerticalTimeline from "vue-vertical-timeline";

Vue.use(VerticalTimeline);
```

and then import it in your `nuxt.config.js` file

```js
plugins: ["~/plugins/vue-vertical-timeline.js"];
```
## Props
 
 This is a list of properties that you can use.

| Property name       | Type    | Default   | Description                                                                                    |
| ------------------- | ------- | --------- | ---------------------------------------------------------------------------------------------- |
| items               | Array   | null      | Array of objects to be displayed.                                                              |
| item-selected       | Object  | {}        | Object that is set when it is clicked. Note that `clickable` prop must be set to true          |
| title-attr          | String  | 'title'   | Name of the property inside the objects, that are in the items array, to set the cards title   |
| title-centered      | Boolean | false     | Centralizes the cards title                                                                    |
| title-class         | String  | ''        | If you want to set a custom class to the cards title, set it here                              |
| title-substr        | String  | 18        | Number of characters to display inside the cards title. Above this, will set a '...' mask      |
| content-attr        | String  | 'content' | Name of the property inside the objects, that are in the items array, to set the cards content |
| content-centered    | Boolean | false     | Centralizes all the cards content text                                                         |
| content-class       | String  | ''        | If you want to set a custom class to the cards content, set it here                            |
| min-width           | String  | '200px'   | Min-width of the timeline                                                                      |
| min-height          | String  | ''        | Min-height of the timeline                                                                     |
| timeline-padding    | String  | ''        | Padding of the timeline                                                                        |
| timeline-border     | String  | '#E9E9E9' | Border color of the timeline                                                                   |
| timeline-background | String  | '#E9E9E9' | Background color of the whole timeline                                                         |
| line-color          | String  | '#03A9F4' | Color of the line inside the timeline                                                          |
| clickable           | Boolean | true      | Makes the card clickable that returns the object                                               |


## Development


Fork the project and enter this commands in your terminal

```sh
 git clone https://github.com/YOUR_GITHUB_USERNAME/vueVerticalTimeline.git
 cd vue-Vertical-timeline
 yarn
```


## License
MIT
