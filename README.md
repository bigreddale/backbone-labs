# Backbone.js Labs

## Models

### Getting Started

1. Navigate to a page which has Backbone loaded.
1. In the Chrome console, create a new Product class.
   We'll keep it simple: no attributes.
   
   ```
   var Product = Backbone.Model.extend({});
   ```

1. Now instantiate this Product, passing in some instance properties.

    ```
    var p1 = new Product({name: 'Beans', brand: 'Heinz'});
    ```

1. How do you view the attributes of this model?
   - Get and set attributes to verify your understanding.
   - Does adding new attributes succeed?
1. Define the class again, this time adding some _default_ attributes.
1. Verify that these are accessible too.

### Implementing a Model Class

1. Extend the Model class to create a Product model class.
1. The class should contain a product name, description,
   productId and image url.
