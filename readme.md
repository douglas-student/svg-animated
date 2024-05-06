# ANIMATED SVG

## Preface

Welcome to the world of Animated SVGs! In this project, I intend to explore and provide a glimpse into the fascinating universe of Scalable Vector Graphics (SVG) and how they can be animated to create dynamic visual content. SVG is a powerful technology for creating vector graphics on the web, and when combined with animation, it opens up a world of possibilities for creating dynamic and interactive visual content.

Throughout this project, I aim to provide several simple examples, bridging the gap between the world of digital designers and the soul of a programmer.

Enjoy! Just as I'll enjoy developing this project.


## Summary

- [TAG ANIMATE](#tag-animate)

## TAG ANIMATE

The `<animate>` tag is one of the most powerful features of SVG for creating animations within vector graphics. With this tag, it's possible to animate attributes such as position, size, color, and shape of SVG elements.

### SUMMARY ABOUT THE TAG ANIMATE

The `<animate>` tag allows specifying initial and final values of an attribute of an SVG element, as well as the duration and type of animation. It can be used to create a variety of effects, from simple animations like translation and rotation, to more complex animations like gradual changes in shape and color. Combined with other SVG tags and elements such as `<path>`, `<circle>`, `<rect>`, among others, `<animate>` enables the creation of dynamic and engaging animations in vector graphics, expanding the possibilities of interactivity and visual expression in web applications and design projects.

## Embedding External SVG

<img src="./svg/campfire-animate/campfire-svg-tag-animate-plano.svg" type="image/svg+xml" width="200" height="300" />

Below is the embedding of an external SVG using the `<object>` tag:
```html
<object data="./svg/campfire-animate/campfire-svg-tag-animate-plano.svg" type="image/svg+xml">
  Your browser does not support SVG
</object>
```

Replace "capfire-svg-animate.svg" with the correct path to your external SVG file

## Animated SVG Code

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 200 300">
  <!-- Background of the Bonfire (wood logs) -->
  <rect x="70" y="200" width="60" height="60" fill="#8B4513"/>
  <rect x="50" y="220" width="100" height="40" fill="#8B4513"/>
  <rect x="30" y="240" width="140" height="20" fill="#8B4513"/>

  <!-- Bonfire Flame -->
  <g id="chama">
    <!-- Initial Flame Path -->
    <path id="path1" d="m 100,84.112338 c 20,35.296132 40.91419,103.783342 0,105.888382 -38.91772,0.71997 -20,-70.59225 0,-105.888382" fill="#ffcc00" opacity="0.8" style="stroke-width:0.939363">
      <animate attributeName="d" dur="2s" repeatCount="indefinite" 
               values="m 100,84.112338 c 20,35.296132 40.91419,103.783342 0,105.888382 -38.91772,0.71997 -20,-70.59225 0,-105.888382;
                       m 100,70 c 16.66667,36.66667 35.99093,109.2646 0.87631,111.71163 C 66.892902,184.07982 83.333333,106.66667 100,70" />
    </path>
    <path id="path2" d="m 100,70 c 16.66667,36.66667 35.99093,109.2646 0.87631,111.71163 C 66.892902,184.07982 83.333333,106.66667 100,70" fill="#ff6600" opacity="0.6">
      <animate attributeName="d" dur="2s" repeatCount="indefinite" 
               values="m 100,70 c 16.66667,36.66667 35.99093,109.2646 0.87631,111.71163 C 66.892902,184.07982 83.333333,106.66667 100,70;
                       m 100,56 c 13.33333,33.33333 34.19773,105.5191 0.83991,105.96756 C 68.313945,176.40483 86.666667,103.33333 100,56" />
    </path>
    <path id="path3" d="m 100,56 c 13.33333,33.33333 34.19773,105.5191 0.83991,105.96756 C 68.313945,176.40483 86.666667,103.33333 100,56" fill="#ff3300" opacity="0.4">
      <animate attributeName="d" dur="2s" repeatCount="indefinite" 
               values="m 100,56 c 13.33333,33.33333 34.19773,105.5191 0.83991,105.96756 C 68.313945,176.40483 86.666667,103.33333 100,56;
                       m 100,42 c 10,30 30,95 0,95 C 70,193 90,120 100,42" />
    </path>
  </g>
</svg>
```
