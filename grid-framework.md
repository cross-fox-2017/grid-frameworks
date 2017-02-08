# Grid Systems
## Jeet

Jeet grid system is dynamic. We can set it to be a 12 column grid or 24 column grid even 5! ```column(1/12), column(1/24), column(1/5)```To make a responsive web design & semantic HTML5 markup with jeed is easy and clean. Example code is provided below.

Bootstrap
```
<div class="container-fluid">  
  <section class="row">
    <aside class="col-md-4">Sidebar</aside>
    <article class="col-md-8">Content</article>
  </section>
</div>
```
Jeet
```
<section>  
  <aside>Sidebar</aside>
  <article>Content</article>
</section>  
```
```
section {  
  @include cf();
}
aside {  
  @include column(1/3);
}
article {  
  @include column(2/3);
}
```

You can see the difference if were using Jeet Grid System the code is more cleaner. We can just set the column straight to the element in HTML. Jeet can use 2 css preprocessor scss and stylus. I personally try to learn and use Jeet grid system in my future project.
[Jeet Official Github provided with documentation](https://github.com/mojotech/jeet "Google's Homepage")

## Mueller

Mueller is a modular grid system. Modular grid is a grid that has consistent horizontal divisions from top to bottom. Mueller grid is for responsive and adaptive website. Adaptive means a fixed grid that was designed for multiple device. While responsive is a flexible width according to the device width. But I personally don't like it because it similar to Bootstrap. The differences is that Mueller has full control over width, gutter width and baseline grid. You can use with compass or Sass preprocessor.

## Responsive Grid system

Responsive Grid system it's nearly the same with Bootstrap Grid System. The differences is just the name of the class and we can set the margin between the column which we can also do in Bootstrap. Example code is provided below

Bootstrap
```
<div class="col-sm-6">
<div class="col-sm-12">
```

Responsive Grid System
```
<div class="col -span_1_of_6">
<div class="col -span_1_of_12">
```

## Gridiculous

Gridiculous it's also the same with Bootstrap Grid System only the class name differences and instead of using ```md, sm, lg``` in bootstrap we use ```grid w960, grid w320``` in Gridiculous. Example is provided below if we want to make 8 columns for the main content and 4 columns for the sidebar.

Bootstrap
```
<div class="col-md-8">
  <div class="row">
  </div>
</div>
<div class="col-md-4">
  <div class="row">
  </div>
</div>
```
Gridiculous
```
<div class="grid w960">
	<div class="row">
		<div class="c8"></div>
		<div class="c4 end"></div>
	</div>
</div>
```

## Unsemantic

Unsemantic it's just the same with Gridiculous and Bootstrap only the class name difference. Unsemantic is the successor from the 960.gs (The first grid system for open source)

## Bourbon NEAT

Neat Grid system is nearly the same with Jeet Grid Systems. You can see the code example below

```
<section>
  <header>What is it about?</header>
  <section>Neat is an open source semantic grid framework built with Sass…</section>
</section>

// Enter Neat
section {
  @include outer-container;
  header { @include span-columns(3); }
  section { @include span-columns(9); }
}
```
The documentation is preety *Neat* you can see it in [here](http://thoughtbot.github.io/neat-docs/latest/) and examples website [here](http://neat.bourbon.io/examples/).
I personally wanted to try this after using Jeet because the HTML code is much more cleaner.
