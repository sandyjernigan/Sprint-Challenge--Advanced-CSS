## Description

The client for this challenge is _Spacewalkers Magazine_. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

[Click here to review the home design](design-files/home-desktop.png)

[Click here to review the mobile design](design-files/home-mobile.png)

## Self-Study Questions

1. What is the difference between an adaptive website and a fully responsive website?

> An adaptive website will adapt to the different screen sizes predefined. However, it is still limited by the defined screen sizes. A fully responsive website, uses the same kind of idea of the adaptive website to create a user-friendly page by using flexible grids and images as well as queries to scale the page to the different screen sizes. Therefore a responsive website only needs one template for all devices that scales, whereas adaptive websites require templates for each predefined size.

2. Describe what it means to be mobile first vs desktop first.

> Mobile First works from the styling with the smallest viewport first increasing to designs for the largest viewport. This is generally seen in css using min-width for the media queries. Whereas, desktop first uses max-width in the media queries. Desktop first focuses on what the webpage will look like on a desktop and work down to smaller sizes and how they will be viewed.

3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?

> It will help to standardize the rem numbers so you do not have to make several calculations. The font-size 62.5% of a 16px standard html font size will convert this to 10 px for the baseline font-size. By converting to 10px baseline you can calculate the rem easier. Now, 1.6 rem will equal 16px.

4. How would you describe preprocessing to someone new to CSS?

> Depends on the audience. 
> For an audience new to coding and with some CSS exposure, preprocessing is a way to both simplify and advance your css. It will simplify the css by allowing you to nest your settings together so that it is easier to read and follow. It also advances your css by allowing you to use the same setting multiple times thru your css using a variable so if you need to change that setting you will only have to change the setting on that variable. This is not limited to just 1 setting either, you can also make setting that you repeat in your code into a predefined setting that you can refer back to and reuse.

>For an audience with coding background, preprocessing is a way to code and compile your css. This uses a few of the same concepts as javascript, C++, and other coding languages, by using variables within the css settings. It will also help to 'DRY' the code a bit by allowing you to nest items and create 'mixins'. This will allow you to make a setting that can be reused, somewhat like a function.

5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

> I really like being about to use variables and escaped strings that can be reused and easily changed. Parametric mixins are really awesome as well, coming from working with php and excel macros these remind me of functions. The concept that gives me the most trouble is just keeping the right order and syntax, like making sure the parenthesis or semicolon are in the right place. 

## Project Set Up

Follow these steps to set up your project:

### Git Set up

- [ ] Create a forked copy of this project.
- [ ] Add your project manager as collaborator on Github.
- [ ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ ] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: git push origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ ] Add your project manager as a reviewer on the pull-request
- [ ] Your project manager will count the project as complete by merging the branch back into master.
 

### Preprocessor Set up

* [ ] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [ ] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [ ] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [ ] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [ ] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [ ] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [ ] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [ ] Add a viewport meta tag to the head of your index.html page

* [ ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [ ] Navigation Styles: Use the `navigation.less` file for styling.

* [ ] Main Content Styles: Use the `home-page.less` file for styling

* [ ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [ ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [ ]  Use at least 2 parameters to create your button

* [ ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [ ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [ ] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [ ] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription