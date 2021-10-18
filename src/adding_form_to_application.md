# Adding a form to our application

* Create a new component using shell command “ng generate component HeroForm”.
* Display the component in the main view and pass a function property onSubmit to it.
* onSubmit function should accept the event from the form and parse it in effect getting the
form values.
* Once the name value is present, a new Dog object with the new name should be pushed to
the doggos array.
* The form itself should have a form tag accepting the submit event, like in the example
below.
* Exercise time!

```ts
<form (ngSubmit)="onSubmit()">
         <label for="name">Name</label>
         <input name="name" id="name">
</form>
```