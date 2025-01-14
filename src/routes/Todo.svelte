<script>
let todoItem = $state('');
let todoList = $state([]);

function addItem() {
     todoList.push(todoItem);
}

$inspect(todoList);

</script>
<form onsubmit={addItem}>
<input type="text" bind:value={todoItem}>
<button type="button">Add</button>
</form>

<style>

</style>