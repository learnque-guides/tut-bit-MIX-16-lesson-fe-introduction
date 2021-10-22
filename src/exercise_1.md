# Exercise 1

* Add an onInit hook in your CategoryComponent.
* On component init, a function named `getSubjects(): Promise<Subjects>` should be called from subject serivce in catgory folder. You need to have in category folder a subjects service. `Subjects` is a type alias for array of string.
* The function should provide us a promise with list of sibjects. You need to add promise callback to get list of subjects and assign them to list of subjects (`public subjects: Subjects = []`;) and set its value to `this.subjects` in category component. `Subjects` is a type alias for array of strings.
* Don't forget to still initialize `this.subjects` as an empty array in the beginning of your component!
* Don't forget to apply changes for category component template (if you need to do that).

---

* Add an onInit hook in your `BooksComponent`.
* On component init, a function named `getBooksSubject(): Promise<Books>` should be called from books service in catgory folder. You need to have in category folder a books service. `Books` is a type alias for array of Book.
* The function should provide us a promise with list of books. You need to add promise callback to get list of books and assign them to list of books (`public books: Books = [];`) and set its value to `this.books` in books component. `Books` is a type alias for array of Book.
* Don't forget to still initialize `this.books` as an empty array in the beginning of your component!
* Don't forget to apply changes for books component template (if you need to do that).
