# Reservations (WaitOnMe App)

This module books table reservations by date and time.

## Related Projects

- https://github.com/table-for-five/header.git
- https://github.com/table-for-five/photos.git
- https://github.com/table-for-five/menu.git
- https://github.com/table-for-five/overview.git

## Table of Contents

1. [Usage](#Usage)
1. [Requirements](#requirements)
1. [Development](#development)

## Usage

> This app places a React application in the global window object under the name 'reservations'.

To get started:

- Install dependencies (see below)
- (Optional) seed database with placeholder reservations:

```sh
npm run mysql-seed
```

- In a static index.html page, include the following:
  - A script tag which invokes ReactDom.render on 'reservations'
  - A script tag with source http://localhost:3003/public/bundle.js

## Requirements

An `nvmrc` file is included if using [nvm](https://github.com/creationix/nvm).

- Node 6.13.0
- Nodemon
- Webpack

## Development

### Installing Dependencies

From within the root directory:

```sh
npm install -g webpack
npm install -g nodemon
npm install
```

### Dev Environment

Run webpack to transpile to server's entrypoint:

```sh
npm run pack
```

### Testing

This application uses the Jest framework with Enzyme library for testing:

```sh
npm run test
```
