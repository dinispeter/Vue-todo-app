<template>
   <div id="app">
     <h1>My Todo App!</h1>
	 <br />
     <TodoList />
   </div>
</template>

<script>
import TodoList from "./components/TodoList.vue";
export default {
  components: {
    TodoList
  }
}
</script>

<style>
*, *::before, *::after {
	box-sizing: border-box;
}

#app {
	max-width: 400px;
	margin: 0 auto;
	line-height: 1.4;
	font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

}

h1 {
	color: #006699;
	text-align: center;
	font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
	font-weight: 200;

}
</style>
