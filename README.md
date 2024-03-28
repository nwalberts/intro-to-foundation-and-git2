# CSS Frameworks

The aim of frameworks in general is to provide a common structure so that developers don’t have to redo it from scratch.

CSS frameworks:
- allow for quicker and easier styling
- provide a cohesive, semi-polished look right off the bat
- are super easy to install!
- help with mobile-friendly layouts

# CSS Frameworks

The aim of frameworks in general is to provide a common structure so that developers don’t have to redo it from scratch.

CSS frameworks:
- allow for quicker and easier styling
- provide a cohesive, semi-polished look right off the bat
- are super easy to install
- help with mobile-friendly layouts
- **Nowadays, primary benefit is their easy to use grid-system

#### What do frameworks provide?
- A grid system
- Nicer typography
- A basic color scheme (which you can mess with!)
- Pretty styling on things like buttons, nav bars, forms, etc.
- Helper classes for things like aligning text

###### *Word of warning: Don't let frameworks be the only styling you do! If you're lazy, your website will look very generic!*

## What frameworks are there?
- **[Foundation](http://foundation.zurb.com/)** (preferred)
- [Bootstrap](http://getbootstrap.com/)
- TAILWIND
- Many, many others

## How to use Foundation

1. First, [download it here!](https://get.foundation/sites.html)
2. Copy css/foundation.min.css into your project's stylesheets folder
3. Link to the stylesheets from your layout.erb file **in this order:**
  * foundation.min.css
  * your own stylesheets!

Bam! You're up and running!

Just by having it installed, Foundation gives you a whole new look - but don't stop there!

#### Some Resources:
**[Foundation documentation](https://get.foundation/sites/docs/index.html):**
This will become your new best friend! All the tools are explained with examples via the bar on the left - browse through to get a sense of what Foundation can do for you. Example code abounds - use it!

**[Foundation templates](https://get.foundation/templates.html):**
Mostly use these as inspiration for how to use Foundation. Don't go copying an entire page of code from here - that'll just make you lazy! If you find a piece of a page you really like, use their code to learn how they use the Foundation tools to make it happen.

**Inspect Element:**
You should be using this all. The. Time. Right click the webpage and hit "Inspect Element", or use Cmd + Opt + I. Click on an HTML element to see the styling that is applied to it!

#### The [Foundation grid system](https://get.foundation/sites/docs/xy-grid.html)
This allows you to use HTML classes to format the layout of your page! By adding `class="blah"` to your HTML element, you get all the nice formatting that Foundation provides for that class.

Foundation imagines that every element of the page is divided into rows and columns. This allows you to specify what sort of space you want your content to take up! You can add rows all you want. For columns, Foundation divides every element into 12 imaginary units of space - you use this to specify what width you want your elements.


Here are some of the classes you'll use:
- `grid-x`: marking something as a row will cause it to take up the full width of its parent element. Use this to mark out a space for vertical elements to reside inside.
- `cell` or `columns`: Preferably use this to wrap your actual content. This will create a column of a certain width (see below) that your content will reside inside.
- `small-#`: This is how you pick how wide your columns are. Remember, every parent element is divided into 12 imaginary units. `small-#` specifies how many of those units you want your column to take up. If I write `small-3`, my column will be 3 units wide, or 25% the width of the parent element. `small-12` will take up the full width of my parent element.
- `medium-#`, `large-#`: the "small" part of the above class means "with small screens, do this". Here you can specify different widths for medium and large screens! This will mean your layout changes depending on screen size. (Yay mobile-friendly design!)

Check out the [docs](https://get.foundation/sites/docs/xy-grid.html) for more useful classes like offsetting your rows, centering columns, etc.

## Git 
- use Git to track what you do in an app since pulling it down
- `git init`
- then open up the source control menu in VSCode, add all changes, and commit
- from now on, every subsequent change you make will be recorded!