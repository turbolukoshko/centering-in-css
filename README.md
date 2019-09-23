# Centering in CSS #

## Support IE8+ ##
1. The parent `<li class="list__item absolute">` needs to specify `position: absolute`, and the child `<div class="list__block">` needs `position: relative`, and also align the contents with `margin: auto`, and `top: 0`, `left: 0`, `right: 0` `bottom: 0`.
2. Percentage alignment of the child `<div class="list__block">` `position: absolute` inside the parent `list__item wooden` `position: relative`. To make child content centered `<div class="list__block">`, you need to raise it half up height `margin-top` and move it left halfway width `margin-left`.
## Support IE10+ ##
3. Alignment with CSS3. The parent `<li class="list__item modern">` needs to specify `position: absolute`, and the child `<div class="list__block">` needs `position: relative` and `top: 50%`, `left: 50%`. To center the child content inside the parent, use the CSS3 property `transform: translateX(-50%) translateY(-50%)`.
4. Centering with Flexbox. We set the following properties for the parent element `<li class="list__item flex">` - `display: flex`, `justify-content: center`, `align-items: center`.