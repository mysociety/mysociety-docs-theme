# mysociety-doc-theme

Templates and sass files for mySociety Jekyll projects.

Intended to be included as a submodule.

## Setting up

The simplist thing to do is to include these as a `theme` directory underneath your current jekyll site.

Add soomething along the lines of the following to `_config.yml`:

```yml
layouts_dir: theme/_layouts
includes_dir: theme/_includes
sass:
    sass_dir: 
    load_paths:
        - theme/sass
        - sass  
```

A layout of 'default' will give a generic mySociety look. 

## Notes

This is not a 'theme' as jekyll knows it, and a local `_includes` does not override the contents of the theme directory. You also can't currently have multiple layouts and includes directories.

If it is not appropriate to just update or add new templates to the shared repo, you can copy all the files up to a higher level and use the same approach.

In the long run, configuring this as a gem-based theme that can be overriden would be the same to fix this - but this approach works for now. 
