# \<icon-rate\>

Polymer element that display rating values using icons.

You can use the iron-icons icon set or a custom one.

## Demo

See [icon-rate](http://altfuns.github.io/icon-rate/demo/) in action.

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower i icon-rate -S
```

## Use it

```html
<icon-rate rate="3.5"></icon-rate>
```

To change the style of the filled and empty icon you can use the `--icon-rate-filled` and `--icon-rate-empty` css mixins.

```html
<style is="custom-style">
  .red {
    --icon-rate-filled: {
      color: var(--paper-red-900);
    };

    --icon-rate-empty: {
      color: var(--paper-red-200);
    };

  };
</style>
<icon-rate rate="4" icon="icons:favorite" class="red"></icon-rate>
```

## Attributes

Attribute     | Options     | Default              | Description
---           | ---         | ---                  | ---
`end`         | *number*    | 5                    | The end value of the rating range.
`icon`        | *string*    | icons:star           | The name of the icon to use. The name should be of the form: iconset_name:icon_name.
`rate`        | *number*    | 0                    | The value of the rate to display. The value should be a number between start and end
`start`       | *number*    | 0                    | The initial value of the rating range
