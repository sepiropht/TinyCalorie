# calorie
Simplest possible calorie counter, as a web-app. Rust (back) + HTML/CSS/vanillajs (front).  
No frameworks! Very fast.

## Dockerfile

You can use the provided dockerfile for easier deployment.
This will expose it on port 8080, and store the SQLite db.db in /path/to/storage.

```bash
docker build -t calorie .
docker run -p 8080:80 -v /path/to/storage:/storage calorie
```

## Features

 - [x] Daily calorie counter
 - [x] Fuzzy search in history
 - [x] Budget/metabolism with weight tracking
 - [x] Very simple UI, quick to add/manage food items
 - [x] Mobile support, fully responsive
 - [x] Activities as negative calorie spending
 - [x] Calendar showing weight loss
 - [x] Browse history through calendar (and add items if forgotten)

## Want

 - [ ] Edit name of items (content-editable?)
 - [ ] Internationalization

## Doesn't want

 - Plugging complex food APIs to find how much calorie is a food, use the numbers at the back of the product, or infer it yourself.
 - Cluttering the interface

## Screenshot

![screenshot.png](screenshot.png)
