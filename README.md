# office-ui-fabric-rails

office-ui-fabric-rails integrates the [Office UI Fabric](https://github.com/OfficeDev/Office-UI-Fabric) framework from Microsoft into the Rails Asset Pipeline

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
//= require jquery.fabric
```

For information on how to use the Office UI Fabric framework see the [documentation](http://dev.office.com/fabric)

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/office-ui-fabric-rails.

For issues with Office UI Fabric itself please use https://github.com/OfficeDev/Office-UI-Fabric

## License

The [Office UI Fabric](https://github.com/OfficeDev/Office-UI-Fabric) framework and the rest of the office-ui-fabric-rails project are licenced under the [MIT License](https://opensource.org/licenses/mit-license.html)


