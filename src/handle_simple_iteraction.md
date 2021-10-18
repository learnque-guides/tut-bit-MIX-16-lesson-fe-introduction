# Handling simple user iteraction (Angular)

 The code below showcases how a simple interaction can be handled – an onClick function triggered by template will add a new doggo to the list. Now, how to adjust this code to fetch a random name from the array?

 ```ts
import {Component} from '@angular/core';

@Component({
  selector: 'app-root',
  template: `
    <div><span>{{dogName}}</span>
      <button (click)="onClick()">Change name</button>
    </div>`,
  styleUrls: ['./app.component.scss']
})
export class AppComponent {
  dogName = 'Alfred';
  goodNames = ['Alfred', 'Joe', 'Friend'];

  onClick() {
    this.dogName = this.goodNames[1];
  }
}
 ```