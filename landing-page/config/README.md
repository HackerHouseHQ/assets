# Configuration types

## Projects

The expected structure of a project is:

```ts
type Project ={
  // Name of the project
  name: string;
  // description for the project
  description?: string;
  // The project's website, portfolio, etc. if they have one
  url?: string;
  // A logo for the project. If missing the project won't show in the carousel
  logo: string;
}
```
