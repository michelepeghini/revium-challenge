# revium-challenge

## NOTES TO ASSESSOR
This is a very basic implementation, which makes use of hardcoded data and local images. It took me 4h to implement.
In the next 2/3 days I would like to add fetching of images via Unsplash API using Axios and state management with VueX, sorry I did not have time to do it outright.

UPDATE: added **composition-api** branch, which makes use of the setup function.

So far, I have made the following components:

---

1. ### Header
Basic stycky header, no responsiveness implemented.

---

2. ### ImageSlider
A wrapper for **vueper-slides** component. For simplicity I decided to use a pre-made slider for Vue3. See [vueper-slides](https://github.com/antoniandre/vueper-slides) repo.

PROS:
- it saves time
- it is highly configurable

CONS:
- it introduces a thrid party dependency

Rationale for choosing this slide rather than another:
- high number of total downloads, 
- high number of weekly downloads, 
- 0 dependencies
- frequent releases

The above factors indicate that the dependency is reliable, flexible and **well maintained**

Additionally: 
- I have made use of soem breakpoints to provide a minimunm of responsiveness.
- The slides' title and content can render HTML which is useful if content was coming from a CMS

--- 

3. ### IntroText
This is a simple component with title and content. 
There is some basic responsiveness for the width of the component.
For simplicity I have used the *data* property of the view to hold text data, but I made use of the *v-html* directive to render the html tags present in the title and content strings. This would be useful if the content was coming from a CMS.

---

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your unit tests
```
npm run test:unit
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
