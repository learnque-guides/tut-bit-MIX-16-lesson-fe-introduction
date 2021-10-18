# Adding attribute type

* Since Angular is written in TypeScript, it assumes that type validation should be present when any data manipulation is done. For that reason, separate classes representing types should be created for your custom types of data. Of course, generic types like string, integer and array are supported by default.

```ts
export class DogType {
    name: string;
}
// or even better???

export type DogType = {
    name: string;
}
```

* For now, our Dogs should probably just have names – let’s assume they are of string type, and thus let’s create a separate file in our working directory named types.ts and put this code in there.