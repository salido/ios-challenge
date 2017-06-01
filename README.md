# SALIDO iOS Challenge
This challenge is intended to get a better idea of a SALIDO candidate's coding style and development process. There is no hard time limit, but we ask that you send in your solution promptly.

Please feel free to use the developer reviewing your work as a resource. If any points seem vague or need clarifying, they will be there to help.

## Submission Instructions

1. Complete the challenge according to the instructions below
1. Post your solution to a Github repo. Be sure to include a README file
1. Email a link to your solution repo to: challenge-accepted@salido.com

## Context
Imagine SALIDO is expanding its reach into the wine industry with a new "SALIDO Wine Club" app.  The app will allow users to browse available wines.  We must source product data from the public wine.com API (http://api.wine.com) and display that data in a concise and user-friendly manner.

## Requirements
1. Upon opening the app, the user should be presented with a list of wines sourced from the wine.com API
	- The user should be able to:
		- Sort by name
		- Filter by category
		- (Or do both while maintaining state)
	- Each listed item should display an image of the item and the item name (if no image exists, display nothing)
	- If the API is unreachable (no internet) an error notification should be displayed on every screen
	- The user should be able to quickly add an item to their shopping cart from this screen, without entering the item's detail screen
2. Upon selecting an item from the list, the user should be taken to an item detail screen
	- The item detail screen should display an image of the item (if it exists) and the item's name
	- The item detail screen should display the item's description as returned from the API
	- The item detail screen should allow the user to add a variable quantity of the item to their shopping cart
3. Upon moving to the shopping cart screen, the user should be shown a list of items that were previously added
	- Items in the list should display the item image, item name, and quantity added
	- Items should be displayed in the order they were added to the cart
	- The total of all item quantities should be present somewhere on the screen
	- The screen should allow the user to return to the main catalogue of items
	- The user should be allowed to remove items from the cart
	- The item detail screen should also be accessible from the shopping cart screen by selecting an item
	- No item in the cart can have a quantity of 0
	- If multiple instances of the same item are added, but at different points, the item should appear in the position that the first instance was added, but the quantity should be grouped. For example:
		- Item A was added with quantity 1
		- Item B was added with quantity 2
		- Another instance of item A was added, but with a quantity of 4
		- The expected outcome is:
			- Item A, Qty 5
			- Item B, Qty 2
4. The user should be able to access their shopping cart at any time.

## Expectations
1. You can model data supplied by the API in a way that is simple and makes sense
2. You can take modeled information and create an easily digestible UI around it
3. You can utilize appropriate frameworks to make your code fast, simple, and DRY
4. You can take a set of business requirements from end-to-end, keeping in mind how the user will interact with the final product

## Other Notes
- Your application must be written in Objective-C
- You DO NOT need to:
	- Save the user's session if the app enters the background. If the user presses the home button, his/her shopping cart data will be lost
	- Handle a checkout or payment - asume all items are free
	- Have a fancy UI - you can make the interface as barebones as you'd like
	- Account for screen rotation
	- Account for iPhone displays - focus on iPads in a fixed landscape orientation
- You can:
	- Use any (free) 3rd party frameworks and libraries as you see fit

- While not an explicit requirement, we encourage you to write simple tests for your validations

- Evaluation:
	We are judging your work based on the following criteria:
	- Did you complete all of the base requirements?
	- Did you follow standard coding practices and use an appropriate programming paradigm for iOS development?
	- Did you properly submit the project?
	- Did you use iOS and 3rd party frameworks in an appropriate way?
	- Did your program crash?
	- Is your code "self-documenting"?
	- Is the data retrieved from the API/created by the user modeled cleanly with the appropriate relationships?
