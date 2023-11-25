## Change Text Based on Screen Size
1.  Create both versions in [[HTML]]
```css
<span class="lg-view">See to the right</span>
<span class="sm-view">See below</span>
```
2.  For mobile-first development, show the small view by default and hide the large view
```css
.lg-view {
	display: none;
}

.sm-view {
	display: inline-block;
}
```
3.  Inside the `media query`, reverse the above styles
```css
@media upXs {
	.lg-view {
		display: inline-block;
	}

	.sm-view {
		display: none;
	}
}
```
