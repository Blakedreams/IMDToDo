<script>
let todoItem = $state('');
let todoList = $state([]);

function addItem(event) {
     event.preventDefault();
     todoList.push(todoItem);
     todoItem = '';
}

$inspect(todoList);

</script>
<form onsubmit={addItem}>
<input type="text" bind:value={todoItem}>
<button type="submit">Add</button>
</form>

<ul>
     {#each todoList as item}
          <li>{item}</li>
     {/each}
     
</ul>


<style>

</style>