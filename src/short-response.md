# Short Response Questions

Answer the following questions in 2-4 sentences each. Be specific and use vocabulary from the lessons.

## Question 1: Flexbox Basics

What is the difference between a **flex container** and a **flex item**? How do you make an element a flex container?

**Your Answer:**
A flex container is the parent element that controls how its children elements are laid out using Flexbox. The child elements inside that parent become flex items. You make an element a flex container by adding `display: flex;` to it in CSS.

## Question 2: Main Axis vs Cross Axis

In Flexbox, what is the **main axis** and what is the **cross axis**? How do `justify-content` and `align-items` work with these axes?

**Your Answer:**
The main axis is the direction that flex items flow, which is usually horizontal when `flex-direction` is `row`. The cross axis runs perpendicular to the main axis. `justify-content` controls spacing along the main axis, while `align-items` controls alignment along the cross axis.

## Question 3: Flexbox vs Grid

When would you use **Flexbox** vs **CSS Grid**? Give an example of a layout that would be better suited for each.

**Your Answer:**
I would use Flexbox for one-dimensional layouts, where items need to line up in a row or a column, like a nav-bar. I would use CSS Grid for more two-dimensional layouts that need rows and columns at the same time, like a product gallery. Flexbox is better for arranging content in one direction, while Grid is better for full page or card layouts.

## Question 4: The `fr` Unit

What does the `fr` unit do in CSS Grid? Explain what `grid-template-columns: 1fr 2fr 1fr` would create.

**Your Answer:**
The `fr` unit means a fraction of the available space in a CSS Grid container. In `grid-template-columns: 1fr 2fr 1fr`, the grid would have three columns where the middle column gets twice as much space as the first and third columns. The first and third columns would be equal widths.

## Question 5: Media Queries

What is a **media query** and why are they important for **responsive web design**? Write an example of a media query that applies styles for screens 768px and wider.

**Your Answer:**
A media query is a CSS rule that applies styles only when certain conditions are true, like the screen being a specific width. Media queries are important for responsive web design because they let a page adjust its layout for phones, tablets, and desktops. For example:

```css
@media (min-width: 768px) {
  .product-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}
```


## Question 6: Mobile-First Design

What does **mobile-first design** mean? What are the benefits of taking a mobile-first approach versus a desktop-first approach?

**Your Answer:**
Mobile-first design means writing the base CSS for small screens first, then using media queries to add styles for larger screens. This approach helps make sure the site works well on phones, where space is more limited. It can also make the CSS easier to build because the layout starts simple and becomes more complex as the screen gets wider.
