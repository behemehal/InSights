# InSights
[![VS Code Marketplace](https://vsmarketplacebadge.apphb.com/version-short/behemehal.insights.svg)](https://marketplace.visualstudio.com/items?itemName=behemehal.insights)
[![GitHub license](https://img.shields.io/github/license/behemehal/InSights)](https://github.com/behemehal/InSights/blob/master/LICENSE)

Minimal code stats extension for VScode

See your project details in status bar to motivate yourself

![statusBarGIF](https://raw.githubusercontent.com/behemehal/InSights/master/img/statusBar.gif)

# How to ignore files ?

* Press `Shift+Tab+P or F1` to open commands
* Type `Create InSights Ignore File`
* Now you can change prefences

# .insightIgnore syntax rules

* You can ignore file extensions like *.[fileExtension]
* You can add settings like @[settingName]=[value]
* You have to write all rules line by line without ','(Comma)
* You cannot add comment end of the rule. Example: e.js //Test File
* You cannot add multiple rules to one line
* You are free to delete this comment
* Settings as default
*  - @exploreTimeout=7000      -  Max 25000 Min 2000 Timeout between reports
*  - @noIgnoreNodeModules=false -  Overrides default node_modules ignore
*  - @reExploreTimeout=5000    -  Min 5000 Timeout for reExploring project


# Example .insightsIgnore file

```js
    package.json
    package-lock.json
    .gitignore
    .eslintrc.yml
    .vscodeignore
    LICENSE
    .npmignore
    .travis.yml
    .jshintrc
    gulpfile.js
    license
    *.txt
    @exploreTimeout=2001
    @reExploreTimeout=20000
```

# [License](https://raw.githubusercontent.com/behemehal/InSights/master/LICENSE)

Copyright (c) 2020, behemehal All rights reserved.