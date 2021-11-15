# 1)Responsive Design Ingredients
1. Fluid layouts(vw and vh and use max-width instead of width)
2.  Responsive units(use rem unit instead of px:set 1rem to 10px for easy calculation)
3. Flexible images(use % for image dimenstion with max-width property)
4. media queries (to change styles in certain viewport)

# 2)How rem and max-width work
```css
.test{background-color:red;padding:100px;max-width:1000px}
/* after being small then 1000px .test will have width of device  */

```

# 3)hero section
![Hero section](./screenshot/Hero%20section.png)

**emmet**
section.section-hero>(.hero>(.hero-text-box>(h1.heading-primary))+(.hero-img-box>img.hero-img))

```html
  <section class="section-hero">
        <div class="hero">
          <!-- LEft side of hero -->
          <div class="hero-text-box">
            <h1 class="heading-primary">A healthy meal delivered to your door, every single day...</h1>
            <p class="hero-description">The smart 365-days-per-year 
          <!--Two button section  -->
            <a href="#" class="btn btn--full margin-right-sm">Start eating well</a>
            <a href="#" class="btn btn--outline">Learn more &darr;</a>
               <!-- Deliver meal section -->
            <div class="delivered-meals">
              <div class="delivered-imgs">
                <img src="img/customers/customer-1.jpg" alt="Customer photo" />
                <img src="img/customers/customer-2.jpg"/>....
              </div>
              <p class="delivered-text"><span>250,000+</span> meals delivered last year!</p>
            </div><!-- End of delivered-meals -->
          </div>  <!-- End of hero-text-box -->
          
          <!-- Right side of hero (img) -->
          <div class="hero-img-box">
            <img src="img/hero.png" class="hero-img" alt="Woman enjoying food .." />
          </div>
        </div>
      </section>

```
```css
.btn--outline:hover,
.btn--outline:active {
  background-color: #fdf2e9;
  /* border: 3px solid #fff; */
  box-shadow: inset 0 0 0 3px #fff;/* Trick to add border inside */
}

.delivered-imgs img {
  height: 4.8rem;
  width: 4.8rem;
  border-radius: 50%;
  margin-right: -1.6rem;/* make every img stack of each others */
  border: 3px solid #fdf2e9;
}

```



