<script>
	import ToDoInputForm from "./ToDoInputForm.svelte"
    let firstName = "Alice"
    let lastName = "Watson"

    $: fullName = firstName  + " " + lastName
</script>

<main>
	<ToDoInputForm userName={fullName}/>
</main>

<style>
	main {
        text-align: center;
        padding: 1em;
        max-width: 450px;
        margin: 0 auto;
	}
</style>