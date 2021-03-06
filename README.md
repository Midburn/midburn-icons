## Midburn Icons (Language)

### Installation

#### `npm i`

### Build

#### `npm run generate` (will create font and CSS under `./dist` folder)

### Adding icons

- Add new SVG file to `./svg` folder.
- Build icon library.
- Push changes

### Notes on adding SVGs

- Remove `<title>` tags!
- Remove `fill` style attributes to allow css manipulations from external apps!
- Prefer single path SVGs!
- Not stating width/height will allow setting these props via external CSS.
- State viewBox for shape positioning.

#### E.G - BAD SVG 😕

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 60 60">
    <defs>
        <style>.cls-1{fill:#231f20;}.cls-2{fill:none;}
        </style>
    </defs>
    <title>art car</title>
    <g id="Layer_2" data-name="Layer 2">
        <g id="for_SVG" data-name="for SVG">
        <path class="cls-1" d="M45,38.71a6.39,6.39,0,0,0-3.38,1l-2.57-2.59L46.15,30l-7.07-7.07L41.5,20.5a6.49,6.49,0,1,0-2-2l-2.46,2.46L30,13.85l-7,7-2.38-2.39a6.46,6.46,0,1,0-2,2L21,22.91,13.85,30l7.07,7.07-2.53,2.54a6.4,6.4,0,1,0,2.06,1.94l2.48-2.47L30,46.15l7-7,2.55,2.57a6.41,6.41,0,1,0,5.4-3Zm0-27.17a3.59,3.59,0,1,1-3.58,3.58A3.58,3.58,0,0,1,45,11.54ZM15.12,18.71a3.59,3.59,0,1,1,3.59-3.59A3.59,3.59,0,0,1,15.12,18.71Zm0,30a3.59,3.59,0,1,1,3.59-3.59A3.59,3.59,0,0,1,15.12,48.71ZM42.14,30l-5.09,5.08L32,30l5.07-5.07ZM30,17.86l5.07,5.07L30,28,25,22.91ZM17.86,30,23,24.92,28,30l-5.07,5.07ZM30,42.14l-5.07-5.07L30,32l5,5.08Zm15,6.57a3.59,3.59,0,1,1,3.58-3.59A3.58,3.58,0,0,1,45,48.71Z"/>
        <rect class="cls-2" width="60" height="60"/>
        </g>
    </g>
</svg>
```

#### E.G - GOOD SVG 😇
```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 60 60">
    <path class="cls-1"
          d="M45,38.71a6.39,6.39,0,0,0-3.38,1l-2.57-2.59L46.15,30l-7.07-7.07L41.5,20.5a6.49,6.49,0,1,0-2-2l-2.46,2.46L30,13.85l-7,7-2.38-2.39a6.46,6.46,0,1,0-2,2L21,22.91,13.85,30l7.07,7.07-2.53,2.54a6.4,6.4,0,1,0,2.06,1.94l2.48-2.47L30,46.15l7-7,2.55,2.57a6.41,6.41,0,1,0,5.4-3Zm0-27.17a3.59,3.59,0,1,1-3.58,3.58A3.58,3.58,0,0,1,45,11.54ZM15.12,18.71a3.59,3.59,0,1,1,3.59-3.59A3.59,3.59,0,0,1,15.12,18.71Zm0,30a3.59,3.59,0,1,1,3.59-3.59A3.59,3.59,0,0,1,15.12,48.71ZM42.14,30l-5.09,5.08L32,30l5.07-5.07ZM30,17.86l5.07,5.07L30,28,25,22.91ZM17.86,30,23,24.92,28,30l-5.07,5.07ZM30,42.14l-5.07-5.07L30,32l5,5.08Zm15,6.57a3.59,3.59,0,1,1,3.58-3.59A3.58,3.58,0,0,1,45,48.71Z"/>
</svg>
```



