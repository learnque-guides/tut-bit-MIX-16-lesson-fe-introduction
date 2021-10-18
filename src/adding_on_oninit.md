# Adding an onInit hook to your component

* With following example a (non-existent yet) function myInitFunction() would be called each time the component is about to render.

```ts
@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.scss']
})
export class AppComponent implements OnInit  {
  ngOnInit() { this.myInitFunction(); }
}
```