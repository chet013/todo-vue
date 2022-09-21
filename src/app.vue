<template>
    <div>
        <header class="header">
            <h1 class="header__title">My ToDo list</h1>
        </header>
        <main class="main">
            <div class="todo">
                <div class="todo-list__field">
                    <input type="text" name="taskText" id="task-text" class="todo-list__input">
                    <button class="button todo-list__add-batton" type="button">Add</button>
                </div>
                <div class="todo-list">
                    <div class="todo-list__task-list"> 
                    </div>
                </div> 
            </div>
        </main>
    </div>
</template>
<script>
import { shallowReactive } from 'vue';

  export default {
    name: 'App',
    data() {
        return {
        }
    },
    methods: {},
  };
</script>
<style lang="css">
    .header {
    background-color: rgb(255, 255, 255);
    display: flex;
    padding: 20px ;
    justify-content: space-around;
    align-items: center;
    }


    .header__title {
        /* border: 3px solid rgb(94, 70, 98);
        border-radius: 2px; */
        text-align: center;
        padding: 12px 30px;
    }

    .main {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 440px;
        background-color: rgb(246, 176, 46);
    }

    .todo {
        max-width: 550px;
    }

    .todo-list {
        overflow-y: scroll;
        width: 100%;
        max-height: 200px;
        min-height: 200px;
        border: 1px solid rgb(21, 20, 22);
        padding: 5px;
        border-radius: 3px;
        background-color: rgb(253, 225, 123);
        box-shadow: 0px 0px 40px -4px rgb(0, 0, 0);
    }

    .todo-list__field {
        display: flex;
        justify-content: space-between;
        width: 100%;
        margin-bottom: 5px;
        padding: 5px;
        background-color: rgb(253, 225, 123);
        border: 2px solid rgb(94, 70, 98);
        border-radius: 3px;
        box-shadow: 0px 0px 29px -0px rgb(0, 0, 0);
    }

    .todo-list__input {
        width: 380px;
        height: 25px;
        background-color: rgb(224, 217, 231);
        border: 1px solid rgb(0, 0, 0);
        border-radius: 6px;
    }


    .task {
        display: flex;
        justify-content: flex-end;
        border: 1px solid rgb(0, 0, 0);
        background-color:rgb(231, 229, 217);;
        border-radius: 6px;
        margin: 1px;
        padding-right: 5px;
        padding-left: 5px;
        min-height: 35px;
    }

    .task__text {
        margin-right: auto;
    }

    /* Buttons */

    .button{
        background-color: rgb(205, 158, 92);
        border-radius: 3px;
        font-size: 12px;
        text-transform: uppercase;
        line-height: 2px;
    } 

    .button:hover {
        background-color: rgb(131, 144, 143); 
    }

    .button:active {
        background-color: rgb(255, 255, 255);
    }

    /* .todo-list__add-batton {
        margin-left: auto;
    } */
</style>
