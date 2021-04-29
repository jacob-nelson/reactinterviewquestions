---
layout: default
---

# What is React JS?

* React JS is a front-end JavaScript library developed by Facebook in 2011.
* It follows the component based approach which helps in building reusable UI components.
* It is used for developing complex and interactive web and mobile UI.
* It was open-sourced in 2015. 
* It has one of the largest communities supporting it.

# What are the advantages of using React?

* ## Use of Virtual DOM to improve efficiency
React uses virtual DOM to render the view. 
* ## Gentle learning curve
React has a gentle learning curve when compared to frameworks like Angular. Anyone with little knowledge of javascript can start building web applications using React.
* ## SEO friendly
React allows developers to develop engaging user interfaces that can be easily crawled by various search engines. It also allows server-side rendering, which boosts the SEO of an app.
* ## Reusable components
React uses component-based architecture for developing applications. Components are independent and reusable bits of code. These components can be shared across various applications having similar functionality. The re-use of components increases the pace of development.
* ## Huge ecosystem of libraries to choose from
React provides you the freedom to choose the tools, libraries, and architecture for developing an application based on your requirement.


# What is Virtual DOM

As the name suggests, virtual DOM is a virtual representation of the real DOM. It is a node tree that lists the elements, their attributes and content as Objects and their properties. Each time the data changes in a react app, a new virtual DOM gets created. Creating a virtual DOM is much faster than rendering the UI inside the browser. Therefore, with the use of virtual DOM, the efficiency of the app improves.

# Explain the working of Virtual DOM.

React’s render function creates a node tree out of the React components. It then updates this tree in response to the mutations in the data model which is caused by various actions done by the user or by the system.
This Virtual DOM works in three simple steps.

1. Whenever any underlying data changes, the entire UI is re-rendered in Virtual DOM representation.
2. Then the difference between the previous DOM representation and the new one is calculated.
3. Once the calculations are done, the real DOM will be updated with only the things that have actually changed. 

# What is JSX?

As stated in the official docs of React, 

> JSX provides syntactic sugar for React.createElement( ) function.

JSX is a shorthand for JavaScript XML. This is a type of file used by React which utilizes the expressiveness of JavaScript along with HTML like template syntax. This makes the HTML file really easy to understand. This file makes applications robust and boosts its performance. Below is an example of JSX:

```jsx
render(){
    return (
        <div>
            <h1>Hello World</h1>
        </div>
    );
}
```

**Note:** _We can create react applications without using JSX as well._

```js
const text = React.createElement('h1', {}, 'Hello World');
const container = React.createElement('div','{}',text );
ReactDOM.render(container,rootElement);
```

# Differentiate between Real DOM and Virtual DOM.

| Real DOM                                 | Virtual DOM                            |
|:-----------------------------------------|:---------------------------------------|
| 1. It updates slow.                      | 1. It updates faster.                  |
| 2. Can directly update HTML.             | 2. Can’t directly update HTML.         |
| 3. Creates a new DOM if element updates. | 3. Updates the JSX if element updates. |
| 4. DOM manipulation is very expensive.   | 4. DOM manipulation is very easy.      |

# Is the Shadow DOM the same as the Virtual DOM?
No, they are different. The Shadow DOM is a browser technology designed primarily for scoping variables and CSS in web components. The virtual DOM is a concept implemented by libraries in JavaScript on top of browser APIs.

# What is “React Fiber”?
Fiber is the new reconciliation engine in React 16. Its main goal is to enable incremental rendering of the virtual DOM. Read more.

# What is reconciliation?
The virtual DOM (VDOM) is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM. This process is called **reconciliation**.

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element edited.
```
