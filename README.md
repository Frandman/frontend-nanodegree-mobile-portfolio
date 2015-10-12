## Website Performance Optimization portfolio project

I accepted the chalenge to optimize this online portfolio for speed! I needed to optimize the critical rendering path and make this page render as quickly as possible by applying the techniques i've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).



### Tha's how you can check my work:

####Part 1: Optimize PageSpeed Insights score for index.html

1. Go to [pagespeed insigths] (https://developers.google.com/speed/pagespeed/insights/)
2. Copy the following adress on the form (an exact copy of the code): frandman.github.io/perf
3. Push enter
4. Check the results :)

To achieve this goal i've used gulp, a node package that automates redundat tasks, such as compress images and minify files.
I've also inlined the styles, make some scripts "async" and avoid the use of external fonts.

####Part 2: Optimize Frames per Second in pizza.html

I optimized the frame per second rate following these technics:

1. Reducing the number of dom elements (pizzas to move in background).
2. Avoiding the use of css properties that triggers paint events.
3. Force the creation of layers in order to avoid paint events.
4. Eliminating duplications in code.
5. Avoiding force synchronous layout, throw measuring elements outside loops.

If you want to take a look, download the repo and use chrome dev tools to check the frame rate is under 60 fps.

Hope you like it :)



