#  Splitting your code into components

Currently, our AppComponent handles all the logic – data fetching, displaying, etc. In order to keep it easily maintainable, it should be split into logical parts. Let’s use the Angular input binding to solve this!

Parent template code:

```html
<child-element *ngFor="let element of parentArray"
   [attribute1]="element"
   [attribute2]="otherAttribute">
```

In the given example, Parent component will be used as a container component – the one that handles all the logic. Child component will be used as a presentational component – the one that displays the data. In this case, 2 properties are passed from the parent component.

```ts
@Component({
   selector: 'dog-component',
   template: `<h2>{{attribute1}}</h2><p>{{attribute2}}</p>`
})
export class DogComponent {
    @Input() attribute1: string;
    @Input() attribute2: string;
}
```

Note the @Input() attribute – it is the binding required for the child component to parse the data from the parent. Also note that the properties have their own types - that is a part of validation from TypeScript! In this way we desribe one way binding (from parent to child).