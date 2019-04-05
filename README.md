
# Applying Classes in the DOM

---

1. Load the `index.html` file contained in that repository in your browser. 

Note: the `one` function goes looking for the div by its `id` attribute, then it modifies the `classList` property using the `add()` function on the object that is returned. 

2. Take a look at the `style.css` file. Notice that there's a class in there called `.blue` whose only job is to alter the `background-color` of whatever element it is applied to. Add another class to `style.css`. Call it `.green`, and have it alter the `background-color` to green.
3. Now go back to the `classes.js` file. Write a new function called two underneath one which finds the element with id 'two' and modifies its classList property. Remember to call it from `start`.

Reload the browser. Did the second div change colour?

4. Pick a colour and follow the previous steps to make a third div change to the colour of your choice.

Note: the fourth div in `index.html` has a class already: `invisible`. It's also not on the screen in the browser. There's no `id` attribute, so we can't find it using `getElementById`.

5. Write a new function called `makeVisible`. To find things by class, we need to use `getElementsByClassName` (note the 's'). `getElementsByClassName` returns an array, because there could be many DOM elements with the class `invisible`. The [MDN documentation on `getElementsByClassName`](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByClassName) might be useful here. Because there's only one invisible div, we know it must be element `[0]` in the array that comes back from `getElementsByClassName`.

6. Add the `'visible'` class to the div's `classList` property using the same method as the previous examples.

7. Call the `makeVisible` function from start.

8. Reload the browser. If all has gone well, you should see a fourth div. If not, spend a little time troubleshooting, then reach out for help on slack.

When you're done, make sure you stage, commit, and push your branch back to GitHub.
