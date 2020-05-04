## To-do list done with React

A simple to-do list project using React for TheOdinProject.

The live version can be found [here](https://andreyskopintsev.github.io/react-todo/)

#### Most important lessons learnt:

1)Use of **'bind'** in constructors. After creating a function in a class we must bind it in the constructor like so `this.deleteItem = this.deleteItem.bind(this)` Without it the functions will not work properly. 
It is also possible to use function expressions like so `let deleteItem = () => {body of the function}`. 
In this project **'bind'** was used instead.

2)Difference between **'props'** and **'state'**. 
**'Props'** are akin to variables that you pass to functions. 
In React props can be passed from a parent to a child like so 
```<TodoItem key={item.id} id={item.id} text={item.text} status={item.done} handleCheck={this.handleCheck} editItem={this.editItem} onDelete={this.delObj}/> ```

Here we can see that it is possible to pass functions as well. 'State' on the other hand consists of various changing elements and cannot be passed. However it can be 'lifted up' like in this project, where all the states were stored in `<App />` but were being manipulated in lower levels.

3)How to deploy React apps to GitHub. A very good article on that can be found [here](https://dev.to/yuribenjamin/how-to-deploy-react-app-in-github-pages-2a1f).

