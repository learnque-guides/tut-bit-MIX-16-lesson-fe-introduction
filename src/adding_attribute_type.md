# Adding attribute type

* Since Angular is written in TypeScript, it assumes that type validation should be present when any data manipulation is done. For that reason, separate classes representing types should be created for your custom types of data. Of course, generic types like string, integer and array are supported by default.

```ts
export class DogType {
    name: string;
}

// or even better ???

export type DogType = {
    name: string;
}
```

* It's a good practise in Angular based application to have a properly create data types.