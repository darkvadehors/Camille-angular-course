# 07 - More on components: Nested Component

*Start from [step-06 branch](https://github.com/mazero/angular-course-app/tree/step-06)

**ℹ We'll work on the created component `starComponent` which display the rating with stars**

1. Use this component as a Nested Component into your `product-list.component.html` to replace the `{{ product.starRating }}`
2. Create an `@Input` property called `rating` into the `starComponent`
3. Update the `StarComponent` template to display 5 stars and listen click on them to `console.log` the clicked value.
4. Create an `@Output` property called `ratingClicked` into the `starComponent` which will return the new value of the rating.
5. Listen the created `ratingClicked` event into the `ProductListComponent` to update the value into the component. 
6. Use the magic of two-way binding in Angular by :
    - refactor `ratingClicked` into `ratingChange` into the `StarComponent` (and update all place where this is in use)
    - update the `ProductListComponent` template to use banana in the box `[(rating)]` in the star component custom HTML element

**SOLUTION:** :octocat: [step-07 branch](https://github.com/mazero/angular-course-app/pull/3)

## Next step

[08 - Services and dependency injection](./08%20-%20Services%20and%20dependency%20injection.md)