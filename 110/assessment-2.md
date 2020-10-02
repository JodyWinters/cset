Pick your favorite CSS property so far. Explain what it's used for and all the potential values or units it can take. Why do you like it?

So far I would say that my favorite property is border. You can give multiple different values to the border property including: a color, size of the border and style the border takes. I like the border property because it is a simple property that can drastically change the apperance of your webpage. Also because it is a shorthand, you don't need as much code to accomplish what you want done.


Imagine you are making a website for a restaurant and you need to style the menu options to show that some are spicy or vegetarian or gluten-free. If all the menu options are using the same HTML elements, what CSS selector(s) could you use and why? Show an example.

To choose which menu items you want you could use the class selector to add your CSS to the specificy menu items that have those extra quirks. For example, you could use: .spicy {} class selector to choose each of the items that are spicy, and then you could add your CSS to each one of them at the same time. However this would involve adding the class attribute to the elements in the html document to signify which ones are spicy or which ones are vegetarian.


Style rules sometimes conflict with each other, especially in large projects. Explain the difference between cascade, inheritance, and specificity and how you can use these concepts to organize your CSS.

The idea of cascading is that when your website is being loaded or built, it will look at each of your rules and properties starting at the top and working towards the bottom. Say that you try to set the text on the website to red, if farther down in your stylesheet you express that you want the text to be blue, it will override the previous property of the text being red. In the case of inheritance, anything that is nested inside of a parent element will take on the properties of that parent element. Example:

html
<p>What color is this <span>text</span>?</p>

css
p {
font-color: red;
}

In this case you can see that the span element is nested inside the p element. When you use the p selector to change the text to red, it includes all elements that are nested inside of it. This would meant that the text inside the span element also turned red. Specificity is the concept that one selector has more precedence than another. If you were to use both a type selector and a class selector, the class selector would always win regardless of which property is above the other. As for how they can be useful, when using multiple instances of the same elements you can change them them all to have the same properties general rules, and then use the specificity or cascading concepts to refine the rules on certain parts of the website.
