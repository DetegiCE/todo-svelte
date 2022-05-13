<script>
    export let todo;
</script>

<div>
    <input type="checkbox" checked="{todo.completed}"/>
    <p style="display: inline;">{todo.text}</p>
    <button>x</button>
</div>
