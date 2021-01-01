# blog-template

This is a Beautiful blog template which can be used to post your blogs

Learn about other css reset files
Learn what is boxing

- `!important` this property in css will prevent from overriding the properties.

## Creating the grid :

To create a grid we need to set the `display: grid` and to create a columns use `grid-template-columns: 1fr 1fr 1fr`.

```css
display: grid;
grid-template-columns: 1fr 1fr 1fr;
height: 100vh; /* temp fix */
```

Explanation : The above code will create 3 columns with the 3 equal fraction because of the 1fr here fr means the fraction and

```css
grid-template-columns: /*No 1*/ 1fr /*No 2*/ 2fr /*No 3*/ 1fr /*No 4*/; //here the column value is as commented
/* fr divides in equal fraction and if we give 1fr 1fr 1fr it will divide screen in 3 equal width column  if we want to make the last column half the screen we can just use the 1fr 1fr 2r*/
```

```css
grid-template-columns: /*No 1*/ 1fr /*No 2*/ minmax(
    0,
    8.5in
  ) /*No 3*/ 1fr /*No 4*/;
grid-column: 2/3; /*this is using the above number values*/
```

Explanation: the above code will create 3 columns with minmax(0,8.5in) this means if the screen is equal to the 8.5in or less than it will just show the only minmax() specified column and it will remove the column which 1fr columns from both the sides.

learn minmax() of css.
