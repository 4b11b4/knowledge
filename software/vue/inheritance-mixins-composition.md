# Re-using Logic in Vue Components
https://vueschool.io/articles/vuejs-tutorials/reusing-logic-in-vue-components/

## Inheritance
- Using the 'extends' keyword, we can inherit a child component.
- In this method, only the contents inside the script tags are used.
  - It should be written in a .js file, but .vue can be used.
- Usually in this method, the .js file to be inherited is not meant to be
  able to have any functionality stand-alone.
- Only one component can be inherited via the 'extends' keyword.
- Lifecycle hooks of the child are executed before the parent.

## Mixins
- Functionality from multiple mixins can be used in a single component.
- If there are data or methods with conflicting names, the parent will
  override the child's.
- Mixins also do not have any template or style tags, they are just plain
  javascript.
- Lifecycle hooks of the mixin are executed before the components which
  are using it.
- Mixins can be used globally, but this use case is very specific.

## Composition
- This approach is more "universal" as it is a similar design pattern in any
  other component-based framework.
- In this method, components only do two things:
  - receive props
  - emit events
