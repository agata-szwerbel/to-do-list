# to-do-list
list where you can select and delete completed tasks

## Demo:
https://agata-szwerbel.github.io/to-do-list/

### Description:
You can use this application to add a new task to the list and then you can mark whether the task has already been completed. You can also delete the task.

### Preview:
https://user-images.githubusercontent.com/107425225/189417499-7ee3b802-75d8-4a38-b985-b62eefa97d5c.mp4

### Used technologies:
- JavaScript
- CSS
- HTML
- BEM

### Part of the code:
```javascript
const render = () => {
    let htmlString = "";

    for (const task of tasks) {
      htmlString += `
            <li class = "js-tasks taskList__item"> 
            <button class="taskList__button taskList__button--done js-done">
            ${task.done ? "✔" : ""}
            </button>
            <span class="taskList${task.done ? " taskList__done" : ""}">
            ${task.content}</span>

            <button class="js-remove taskList__button taskList__button--delete">🗑</button>
            
            </li>
            `;
    }
    ```

