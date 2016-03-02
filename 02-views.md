# Backbone Labs

## Views

Navigate to http://backbonejs.org/.
In the console, perform the following:

1. Create a new Product class:

        var Product = Backbone.Model.extend({
            defaults: {
                name: 'Unnamed Product'
            }
        });

1. Also create a ProductView:

        var ProductView = Backbone.View.extend({
          initialize: function () {
            this.render();
          },
          render: function () {
            console.log(this.el);
          }
        });

1. When you instantiate a view, what does it return?
1. Instantiate a view and provide it with properties:

        var p1 = new ProductView({el: 'div'});

    - What happens now?

1. Experiment with adding `className`, `id` and `tagName` to your ProductView.
   How do these affect the rendered result?

## Using a View to Render a Model

The directory` 02-views` contains a skeleton HTML file which:

- loads jQuery, underscore and backbone
- loads `index.js`

1. Update `index.js` to:

    1. Create the Product model class from the previous lab.
    1. Create a ProductView class with the Product model as its `model`
        1. Update its `render()` method to extract the `name` and `brand` properties from the model.
    1. Create instances which render your view into three different elements.
