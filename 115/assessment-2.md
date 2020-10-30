In the next few weeks, we'll be learning how professional developers work on larger projects. What are you most looking forward to in this section?

  From the sounds of the class, it seems like it might give me a normal structure to follow when working on large projects. Up until now the projects have been smaller so where you put your focus and in what order you write hasn't been nearly as important as I think it will become. So I look forward to seeing how professionals handle their workloads.

Briefly explain event propogation and bubbling using an example of two nested HTML elements.

  Example:
  <nav>
    <a href=""></a>
    <a href=""></a>
  </nav>

  Say you were to click on the link that the example above makes. Even though you are clicking the link, you are also clicking into the nav area as well since it is the links parent element. So if you had an event listener on both the link and the nav, when you click the link both event listeners will activate.

You learned to use addEventListener on a DOM node to listen for a type of event and create a function to handle that event. When the event happens, that function is called with an Event Object that gives you more information about the event. Choose two different event types and explain two properties of each that are unique to that event. Use your MDN reference for help.

  The first type I'll use is 'mousedown'. First you can use the detail property to find how many times the mouse was clicked within a short time. Second you can use the 'button' property to find which button on the mouse the user clicked with. The second type will be 'keydown'. You can use the 'key' property with 'keydown' to give you the character that was pressed. For example(event.key) when pressing the "f" key will return f. A second property is 'code'. Using (event.code) will give you a value based on the physical key on the keyboard. Typing "f" with 'code' will give you 'KeyF'.
