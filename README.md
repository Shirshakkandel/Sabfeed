# 1)Responsive Design Ingredients
1. Fluid layouts(vw and vh and use max-width instead of width)
2.  Responsive units(use rem unit instead of px:set 1rem to 10px for easy calculation)
3. Flexible images(use % for image dimenstion with max-width property)
4. media queries (to change styles in certain viewport)

# 2)How rem and max-width work
```css
.test{background-color:red;padding:100px;max-width:1000px}
/* after being small then 1000px .test will have width of  */

```

# 3)hero section
![Hero section](./screenshot/Hero%20section.png)
```css
.btn--outline:hover,
.btn--outline:active {
  background-color: #fdf2e9;
  /* border: 3px solid #fff; */
  /* Trick to add border inside */
  box-shadow: inset 0 0 0 3px #fff;
}

.delivered-imgs img {
  height: 4.8rem;
  width: 4.8rem;
  border-radius: 50%;
  margin-right: -1.6rem;
  /* make every img stack of each others */
  border: 3px solid #fdf2e9;
}

```



