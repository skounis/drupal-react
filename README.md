# Integrate React into Drupal
A working example.

## Quick start
1. Copy `.example.env` into `.env` 
2. Run `ahoy up` 
3. Run `ahoy composer install` 
4. Run `ahoy prepare` 
4. Run `ahoy install` 
5. Visit http://localhost:8080/web

Login: `admin` / `admin` 

## Enable the React module
Symlink the `lib`
- `ln -sr lib web/modules/custom`

Enable the module
- `ahoy drush en mt_react_demo`

### Environment
- Web server: localhost:8080
- PHPMy Admin: localhost:8090
- MySQL: 
    - localhost:3306 || mysql:3306
    - u: `root` p: `none` 

### Shell access
- `ahoy sh`


## References
- [A Recipe for an Embedded React Component in Drupal](https://www.mediacurrent.com/blog/recipe-embedded-react-component-drupal/)
- [Using React library on Drupal](https://www.appnovation.com/blog/using-react-library-drupal)


# How to Send Message
Use the Firestore database in the project
- https://console.firebase.google.com/u/0/project/better-events-drupal/overview

Create `toast` documents by using the structure:
```
{
   body: String
   intention: String // info | success | warn | error | dark
}
```

Example
```
{
   intention: "info",
   body: "Foo bar buzz."
}
```
```
{
   body: "Foo bar buzz."
}
```


