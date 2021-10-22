# Exercise 2

1. In header component pass title (`public title = 'Reading list';`) property that will come from root component (app.component.ts)
2. Implement in category component subject selection logic. You need to add click handler inside dropdown that you have created earlier and pass subject to it (`onChangeSubject`). Selected subject must be displayed in console.
3. In books component you need to implement on click event when pressing on table row. When table row is clicked you need to pass book that is used in this row (`onBookSelect`).
4. From books component pass the  book that you are getting when click action on row in table occur. Replace hardcoded data with concrete book.

P.S. If books are not fetched or book is not selected you need to hide table and book details and show meesage in html that books are loading or book is not selected and it is not possible to show book details. Do not forget about `ngSwitch` and `ngSwitchCase` or `ngIf`