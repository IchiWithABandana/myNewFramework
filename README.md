# myNewFramework
Complete Guide on how to create your framework.

We want to have an easy to use, responsive and structured framework that can be easily modified with multiple themes and templates. We are using Sass to deploy a faster and more efficient styling.

First thing let's make sure that we can access our files with a CDN provider: I fairly advise https://raw.githack.com/ that perfectly serves our purpose here.
- Create a Repositry on Github and make it public.
- Structure your files and upload them to your Repositry.
- Copy the link of your main file and paste it in our CDN provider.
- Select the production link (there are two links… The other one being developement) and copy it.
- paste the element inside your head section withing a link tag in href and Voila!

Now let us structure our files and see what we might need. First things firts, we need to have a grid system that allows us to position the elements inside our website freely. The grid system is set with responsive design that puts all the elements in the good place regardless of the device. Our Grid system is independant and can be applied to all elements making it a major file that is subject to higher hierarchy.

The grid system will contain:
+ .g6 : responsive 6 columns seperator on multiple levels.
    
    Use .g1 to .g6 to seperate the screen, the .g6 is always equal to 100% but others vary depending on screen size. A .g1 is 50% of a mobile device but 16.66% of a large screen.

    Keep in mind that having a .g3 class inside a .g4 class means that the child class is the half of .g4, it means that in a large screen .g4 equals to 66.66% so the .g3 will not be equal to 50% but 33.33%;

+ wrapper : element centering options and margins.

    The .wrap class allows us to center an element depending on its width meaning that the .g6 system is necessary for it to work.
    The varient is the .wrap-1-1 to .wrap-10-10 that allows us to responsively distance elements one from another. Use the bigger wrap to give higher distance to elements.

+ container : responsive padding for block elements.

    Just like the wrapper, the .cont-x-y elements are responsive and gives you the abilitty to control paddings and give your elemetns the best practical use when resizing the window or changing device.

+ position : responsive fixed and absolute elements on use.

    The .fixed and .absolute .relative are used with -lX -tX -rX -bX and can be added up with X[0-100].

+ row :
     The row is mainly the most useful element of this system. It allows you to put elements next to another regardless of there position as long as their added .g1 are not equal to 6: .g3 + .g3 | .g2 + .g4 |….

     To make this possible we set all elements with a bos-sizing of border-box.

The second part of our framework is the themes, it is fairly usefull to make it now so the construction of our framework does not lack of consistency and visual effects. The themes must be seperated from the main content and added just before all other elements. The theme consists of fonts, colors

+ Our themes are composed with two main elements: Colors and Fonts. The themes will be developped afterwords when the rest of the documents are set to be working, the current light theme will display the usual elements.

+ The Elements that we create are all set for the light theme. We have the list elements grouping also the navigation that is totally manipulated by the positioning and cont/wrap combo. It is good looking and very useful. We also have a second element in this section regarding the Tables that allows a similar but authentic feeling.

+ Now we have the form elements: The file uploding files comes with easier set ups allowing better understanding and customizable buttons. All other elements that have displayable styles such as select | input:number and others all have different styling reagarding their usability. It is all set to be a little part of the framework so it is very Light. The Scrollbars are also taken care of to allow perfect layout and branding customization.