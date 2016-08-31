# office-ui-fabric-rails

[![Gem Version](https://badge.fury.io/rb/office-ui-fabric-rails.svg)](https://badge.fury.io/rb/office-ui-fabric-rails)

office-ui-fabric-rails integrates the [Office UI Fabric Core](https://github.com/OfficeDev/office-ui-fabric-core) and [Office UI Fabric JS](https://github.com/OfficeDev/office-ui-fabric-js) frameworks from Microsoft into the Rails Asset Pipeline

## Current Framework Versions

Since this gem was first released, Microsoft have split the framework into two components, the Core framework which contains fonts, colours etc and the JS framework which contains the components such as Breadcrumbs, Buttons etc. These have two different version numbers at present, I may in the future split the gem in two to match what Microsoft have done with the framework, in the meantime the version number of the Gem will track the core framework and I will do minor increments for JS framework updates. I will update this readme with the versions currently being used (Ensure you look at the correct branch for the version you are using)

[Office UI Fabric Core](https://github.com/OfficeDev/office-ui-fabric-core) - v4.0.0
[Office UI Fabric JS](https://github.com/OfficeDev/office-ui-fabric-js) - v1.0.0

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'office-ui-fabric-rails'
```

And then execute:

    bundle

## Usage

### Add Office UI Fabric to your CSS

#### CSS

Add the following line to the end of your `app/assets/stylesheets/application.css` file:

```
*= require fabric
```

If you also wish to use the [Fabric components](http://dev.office.com/fabric/components) then you should also add

```
*= require fabric.components
```

#### Sass

If you are using Sass then you can add the following to your application.scss instead:

```
@import "Fabric";
```

If you also wish to use the [Fabric components](http://dev.office.com/fabric/components) then you should also add

```
@import "Fabric.Components";
```

Or you can just import the components you wish to use from the components directory. The names match those listed on the [fabric site](http://dev.office.com/fabric/components). E.g to include the Breadcrumb component add

```
@import "components/Breadcrumb"
```

### Add Office UI Fabric to your JS

Add the following to your `app/assets/javascripts/application.js` file:

```
//= require fabric
//= require fabric.templates
```

For information on how to use the Office UI Fabric framework see the [documentation](http://dev.office.com/fabric)

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/craigplummer/office-ui-fabric-rails.

For issues with Office UI Fabric itself please use https://github.com/OfficeDev/Office-UI-Fabric

## License

The [Office UI Fabric](https://github.com/OfficeDev/Office-UI-Fabric) framework and the rest of the office-ui-fabric-rails project are licenced under the [MIT License](https://opensource.org/licenses/mit-license.html)


