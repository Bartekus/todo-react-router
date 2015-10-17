React-Router ToDo App
======

ToDo App using (**react-router**) combo and utilizing firebase backend / gulp workflow.

#### Screenshot

![Screenshot software](https://raw.githubusercontent.com/Bartekus/todo-react-router/master/todo-react-router.png "screenshot software")

## Synopsis

Full feature todo list app with persistent data using react-router combo and firebase backend.

## Code Example

```
render: function() {
  return <div className="row panel panel-default">
    <div className="col-md-8 col-md-offset-2">
      <h2 className="text-center">
        To-Do List
      </h2>
      <Header itemsStore={this.firebaseRefs.items} />
      <hr />
      <div className={"content " + (this.state.loaded ? 'loaded' : '')}>
        <List items={this.state.items} />
        {this.deleteButton()}
      </div>
    </div>
  </div>
},
```

## Motivation

Coupling react with router to enable more dynamic operation and the experiance that it provides.

### Directory Layout

```
.
├── /node_modules        # Dependancies source
├── /sass/               # SASS/SCSS folder
│   └── /style.scss      # SASS/SCSS stylesheet
├── /src/                # Source folder
│   ├── /app.js          # App's main loop source
│   ├── /header.js       # Header module source
│   ├── /list-item.js    # List-item module source
│   └── /lisr.js         # List module source
├── .gitignore           # Version control omission file
├── gulpfile.js          # Gulp control file
├── index.html           # Main entry point
├── main.html            # Main App
├── package.json         # Dependencies management file
├── README.md            # This file
└── todo-react-basic.png # Picture
```

## Installation

Checkout this repo, install dependencies, then open index file with the following:

```
  > git clone git@github.com:Bartekus/todo-react-router.git
  > cd todo-react-router
  > npm install
  > gulp (might have to execute: npm install -g gulp)
```

## Usage

Use to add/edit/delete tasks that persist using router and a firebase backend.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

0.1.0 Finalized the example

## Tests

Basic non-automated manual browser test aka no test :P

## Contributors

Standing on the shoulders of all the giants before me.

## Contact
#### Bartek Kus
* Homepage: http://bartekus.com
* E-mail: bartekus@gmail.com
* Twitter: [@Bartekus](https://twitter.com/Bartekus "Bartekus on twitter")

## License

Copyright (c) 2015 Bartek Kus

Licensed under the MIT license
