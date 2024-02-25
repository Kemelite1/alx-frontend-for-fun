# Sass & Scss
Sass is a preprocessor scripting language that is interpreted or compiled into Cascading Style Sheets (CSS). It provides syntax enhancements like variables, nesting, and mixins to make CSS more maintainable and easier to write.
# How to write Sass & SCSS files:
Sass files have a `.sass` extension and use indentation to separate code blocks, while SCSS files have a `.scss` extension and use curly braces {} and semicolons ; similar to CSS.
# Difference between Sass and SCSS:
Sass and SCSS are two different syntaxes for writing Sass code. Sass uses indentation for nesting and omits semicolons and curly braces, while SCSS syntax is more similar to CSS, making it easier for developers familiar with CSS to transition to SCSS.
# Sass preprocessing:
Sass preprocessing involves compiling Sass or SCSS files into standard CSS files that browsers can interpret. This process is typically done using a build tool like Sass CLI, Gulp, or Webpack.
# How to declare a variable:
Variables in Sass/SCSS are declared using the $ symbol followed by the variable name and assigned a value. For example: `$primary-color: #FFF;`
# How to import a Sass file:
You can import other Sass files into your main Sass file using the @import directive. For example: `@import 'variables';`
# How to use nested definition:
Nested definitions allow you to nest CSS selectors within one another, which can improve readability and maintainability.
`nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;

    li {
      display: inline-block;
    }
  }
}
`
# How to declare extend/inheritance styles:
Extend/inheritance allows one selector to inherit styles from another selector. This is done using the @extend directive.
`%message-shared {
  border: 1px solid #ccc;
  padding: 10px;
  color: #333;
}

.success {
  @extend %message-shared;
  background-color: #dff0d8;
}

.error {
  @extend %message-shared;
  background-color: #f2dede;
}
`
# How to manipulate operators:
Sass supports various mathematical operators like +, -, *, /, and % for numeric values. 
`.container {
  width: 100% / 3;
}
`