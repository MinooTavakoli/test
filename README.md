
# Minimap For React

![minimap](https://imageupload.io/ib/tYll9Sh5MEQm18q_1691943250.png)

#### I named this project Minimap!

Minimap is a small web application that displays both a list of vehicles and a map showing all vehicles in the city of Hamburg.
When the user clicks on a specific vehicle in the list, the map zooms to that vehicle's location and somehow shows its location.
Also, clicking on a marker somehow highlights the matching item in the vehicle list, and also centers/zooms the map on it.
And finally, it displays the details of the car in a small pop-up.

- [Run](#Run)
- [UsagePackages](#UsePackages)
- [Files](#Files)
- [Props](#Props)
- [Author](#Author)

### Run

> Use the following command to run the project

```bash
npm run dev
```

### Files

> Project structuring

```bash
File as mock data:
src/constants/vehicles.ts

Display the list of vehicles and the map:
/src/components/map/index.tsx

Certain screen of car details and specifying types:
/src/components/map/components/DetailModal/index.tsx
/src/components/map/components/DetailModal/types.tsx


Display the specified points on the map and the corresponding types:
/src/components/map/components/MArkerList/index.tsx
/src/components/map/components/MArkerList/types.tsx
```

## USE Packages

```bash
yarn create vite map-vite-project --template

why vite?
Fundamentally, at the core, Vite.js does two main things, and does it really well:
Serve code locally during development
Bundle all your frontend assets (HTML, CSS, JS etc.) for production.
Vite leverages native ES modules in the browser. This will help to load your code instantly, no matter how large your module dependencies are or how large the application code has become. Vite also uses Hot Module Replacement (HMR). HMR accounts for the fast and effective part of Vite, as it watches for state changes in the application and adds and/or removes modules while the application is running without prompting a full reload of the application. What this means for the developers is you can see the changes you make to your code instantly right in your browser as you're coding.

yarn add @emotion/react @emotion/styled
why emotion/react & @emotion/styled?
Emotion is a library for styling React applications that provides a simple and efficient way to manage your styles. It allows you to write CSS in JavaScript and provides a flexible API for styling your components.

yarn add framer-motion
why framer-motion?
Framer Motion is a simple yet powerful motion library for React.
It powers the amazing animations and interactions in Framer, the web builder for creative pros. Zero code, maximum speed.

yarn add mapbox-gl
why mapbox-gl?
The "GL" in Mapbox GL JS refers to Mapbox GL, a graphics library that renders 2D and 3D Mapbox maps as dynamic visual graphics with OpenGL in any compatible web browser, without using additional plugins.
Client-side rendering
Mapbox GL JS relies on client-side rendering. Mapbox GL JS maps are dynamically rendered by combining vector tiles with style rules in the browser rather than on a server, which makes it possible to change the maps's style and displayed data in response to user interaction.
```

## Props

| props               | defaultValue      |
| LocationData        | null              |
| setZoomPosition     | 12                |
| setSelectedLocation | LocationData      |

### Author

> Minoo Tavakoli
