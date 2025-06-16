<script>
  import Child from "./component/Child.svelte";
  let name = 'HuXn'
  let age = 23;
  let location = 'china';
  let hobby = 'coding';
</script>

<Child
  {name}
  {age}
  {location}
  {hobby}
/>