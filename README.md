# Ruby Getter Method Modification

This example showcases a common error in Ruby when attempting to modify an object's internal state through its getter method.  The `value` method acts as a getter, providing read-only access to the `@value` instance variable.  Direct assignment through this getter (`my_object.value = 20`) results in a `NoMethodError` because the setter method is not defined.