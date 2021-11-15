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
