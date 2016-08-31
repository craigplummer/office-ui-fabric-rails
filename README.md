# office-ui-fabric-rails

[![Gem Version](https://badge.fury.io/rb/office-ui-fabric-rails.svg)](https://badge.fury.io/rb/office-ui-fabric-rails)

office-ui-fabric-rails integrates the [Office UI Fabric](https://github.com/OfficeDev/Office-UI-Fabric) framework from Microsoft into the Rails Asset Pipeline

## IMPORTANT INFORMATION

As a result of a recent change by Microsoft to split the Office UI Fabric framework into two projects for Core and JS. I have made the decision to split the gem in two - this gem will get no further updates and you should instead use:

[office-ui-fabric-core-rails](https://github.com/craigplummer/office-ui-fabric-core-rails) for the [Office UI Fabric Core](https://github.com/OfficeDev/office-ui-fabric-core) framework.

and

[office-ui-fabric-js-rails](https://github.com/craigplummer/office-ui-fabric-js-rails) for the [Office UI Fabric JS](https://github.com/OfficeDev/office-ui-fabric-js) framework which includes the [Fabric components](http://dev.office.com/fabric/components).

You won't need to make any changes to the includes within your CSS/SASS or JS files after switching to these gems and you will continue to get the latest updates to the framework.

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
@import "fabric";
```

If you also wish to use the [Fabric components](http://dev.office.com/fabric/components) then you should also add

```
@import "fabric.components";
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
