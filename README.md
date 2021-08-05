# Pascetti.css

This project is using the [7-1 architecture pattern](http://sass-guidelin.es/#architecture) and sticking to [Sass Guidelines](http://sass-guidelin.es) writing conventions.

Each folder of this project has its own `README.md` file to explain the purpose and add extra information. Be sure to browse the repository to see how it works.

### Sass conversion

This project uses the .scss convention (because indentation sucks). If you want to use .sass, run the following:

```
sass-convert -F scss -T sass -i -R ./  && find . -iname “*.scss” -exec bash -c 'mv "$0" “${0%\.scss}.sass"' {} \;
```

### Compiling

When using `node-sass` - for building

- install `node-sass` if not yet installed:

```bash
npm install -g node-sass
```

- run build command from command line:

```bash
npm run autocompile-scss 
(or node-sass stylesheets/main.scss dist/main.css)
```

### Resources

https://levelup.gitconnected.com/bundle-a-css-library-6e9ff1ff8a2c
https://geekyants.com/blog/building-your-own-css-framework-373
[Scaling units](https://die-netzialisten.de/em-und-rem-was-ist-der-unterschied/)
[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

[Autocompile Sass](https://mishkaorakzai.medium.com/how-to-add-and-compile-scss-to-run-automatically-in-the-background-on-an-existing-node-js-project-f0172141ae47)
[Find font sizes](https://type-scale.com/)