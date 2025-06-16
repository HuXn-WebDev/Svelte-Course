<script>
   import Child from "./components/Child.svelte";
</script>

<!-- Whenever you wanna pass some content (HTML)
    from parent component, down to the child component,
    you can use the `children` prop.
-->

<Child>
    <h1>Hello World</h1>
    <ul>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
</Child>