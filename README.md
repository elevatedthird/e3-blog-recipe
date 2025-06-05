# Elevated Third Blog Recipe
Contains a recipe for a simple blog using best practices

## Usage
To use add the following to the "repositories" key in your composer.json file:

```json
"e3-blog-recipe": {
    "type": "vcs",
    "url": "https://github.com/elevatedthird/e3-blog-recipe"
}
```

Then run `composer require elevatedthird/e3-blog-recipe` to install the recipe.

Then run `drush recipe /app/recipes/e3-blog-recipe -v` to apply the recipe

## Contributing to recipe
Any configuration added to the config dir will be installed when the recipe is applied.
When pushing updates be sure to add a release tag to ensure composer will pull the new version.

```shell
git tag 1.0.1
git push origin 1.0.1
```