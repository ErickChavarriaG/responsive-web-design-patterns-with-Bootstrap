# responsive-web-design-patterns-with-Bootstrap

I will demonstrate 4 web design patterns using Bootstrap 3:

1. The Mostly Fluid Pattern
2. The Column Drop Pattern
3. The Layout Shifter Pattern
4. Same Sized Columns
 

The Mostly Fluid Pattern - http://aurimas.darguzis.com/projects/Mostly-Fluid-Pattern/ 

  One of the problems we have when we are working with web design and we are going from a multi-column layout down to a single-column layout, is how exactly do we want to stack the columns. There is no hard and fast rule, and it is totally up to the web designer, but in a lot of cases you might want your major content to come first. So instead of showing the left aside column, we would want to list out the articles from middle section. I have setted up three column layout to start with - left-side aside column, middle section for articles and right-side aside column. Now Bootstrap is a Mobile first technology. Things work out better if we arrange things for mobile, and on mobile we are gong to want the middle section to be first. I am going to use col-xx-push and col-xx-pull classes to achieve desired result. 
  
The Column Drop Pattern - http://aurimas.darguzis.com/projects/Column-Drop-Pattern/

There is another pattern called Column Drop. This pattern will drop columns one by one to the bottom of the page as the screen size gets smaller. The columns never go away, instead they just stack up on the bottom of the page. Let's say we want thing to change on the small screen size using our code from fluid pattern. Small screen size would be a tablet and we want just two columns when the webpage is loaded on them. The third - right aside - column will go beneath the left aside column and the middle section.

So for this Column Drop pattern we will have three layouts - one for the extra-small phone size, and then one for the small tablet size, and then anything larger on the medium and large form-factors, we will keep three columns layout.

For the small breakpoint I would like to set the main content to be 9 columns row. And when we get up to the medium breakpoint, I am going to want this to go back to 8 columns. For the extra-small breakpoint this will still just be outside of the grid, it will just take up the full width of the device. For a tablet, it will take up 9 columns, which means that left aside column is going to have to take up 3 columns. And then on the medium size and larger, I would like it to take up 8 columns. And looking at the final column of the right aside, I will set col-sm-2, but just to be clear, you can set col-xs-12 so that way, on the extra-small and larger devices it will take up the full width of the screen, until we hit col-md, in which case we will only take up 2 columns. Just keep in mind that when we jump from extra-small up to medium, we are skipping small, so small is going to take this characteristic of being the full width of the screen. The last thing is left to do is to align the columns accordingly on the medium and large screens. We need to push our middle section off to the left side.

So I will add the class col-sm-push-3. The reason we want to push it 3 grid columns is because our left aside column is going to be 3 grid columns wide at the small lever. Likewise, at the medium level the left aside column is going to be 2 columns wide, so we are going to have to make sure that we have a class col-md-push-2. And we need to pull the left aside column. I want it to always show up on the left side of the screen so I add the class col-sm-pull-9. Right at the small level, our main content (middle section) is going to be 9 columns wide, and at the medium level our content is going to be 8 columns wide. We also need to add col-md-pull-8.

Just keep in mind that when you are working with the Bootstrap grid things can get a little bit confusing, and the key thing to keep in mind is that you always want your elements to add up to 12 columns, so at the small level we have 3-grid coluns, which means our main content needs to take up 9 columns. And then at the medium level our main content is taking up 8 columns, and our left aside column is taking up 2 columns, so we need to make sure that the final column takes up 2 columns for medium. And the other thing to keep in mind is that we always push and pull from the left side of the page. At the small breakpoint we need to push it over to the right three grid columns, and at the medium we only need to push it over 2 columns. And pull is the exact opposite. We want to pull it over 9 columns fro small, and we want to pull the left aside column over 8 columns for large.
  
The Layout Shifter Pattern - 
  the code is on the way :)

Same Sized Columns - 
  the code is on the way :)
