# Development Information

Information about and for the development of Seeking Shelter.

## To do

- [ ] Reorg `src/plot_interactive_geomap.py` to improve build process (currently running some things twice...)
- [ ] Decide whether to use a backend (e.g. places near me...instead of computation on client)
- [ ] Decide whether/which front-end framework to use
- [x] Write About page
- [x] Cluster markers
- [x] Use marker icons that are easily recognisable
- [x] 'Near me' feature
- [x] Add `tel:` hyperlink to telephone numbers in popups
- [x] Make map display mobile friendly
- [x] Zoom to user's location
- [x] Provide separate basic and advanced maps
- [x] Add menu

## Setup

The project is a bit of a mixture of intertwined Python jinja2 and JavaScript React.js... This could be improved.

### Python

```
virtualenv src/env
source src/env/bin/activate
```

Then in the activated environment:

```
pip install -r requirements.txt
```

### JavaScript

```
npm install
```

## Build

### Python

```
source src/env/bin/activate
python src/build.py
```

### JavaScript

```
npx babel --watch src/react --out-dir . --presets react-app/prod
```
