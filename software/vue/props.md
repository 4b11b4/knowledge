# Non-Prop Attributes
https://vuejs.org/v2/guide/components-props.html#Non-Prop-Attributes
https://tahazsh.com/vuebyte-non-prop-attributes
https://www.raymondcamden.com/2018/04/03/til-vuejs-and-non-prop-attributes

1. Say you create a component which simply wraps the <img> tag.
2. You didn't create a prop to allow for 'alt' text, but you still want to
   pass some text for a title. You can simply still pass an attribute to your
   component as expected.
   e.g. <my-component title="alt text here"></my-component>
   - Note that these attributes will be passed to the root element. In other
     words, if your <img> tag is the root element, then the title attribute
     will be passed properly. If you wrap everything in a <div>, then the
     attributes will be passed to the div instead.
3. Instead the attributes being passed to the root element exclusively, we 
   can specify where we want them to go instead.
   e.g. <img
          :src="url"
          v-bind:"$attrs"
        />
   Now if you pass any non-prop attributes to your component, they will go
   into the img instead of the root element (maybe a div for example).
4. $attrs contains all non-prop attributes except class and style. These
   would still be passed into the root element. Vue will combine the classes
   instead of overridding the one defined by the parent.
5. If we want to prevent the root element from inheriting attributes that
   we didn't explicitly define, we can add a field to our component's options:
   e.g. <script>
        export default {
          inheritAttrs: false
        }
        </script>
