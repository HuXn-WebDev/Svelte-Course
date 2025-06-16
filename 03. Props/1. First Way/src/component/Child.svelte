<script>
const { name, age, location, hobby } = $props();
// console.log(name, age, location, hobby);
</script>


<div>
  <h1>Child Component</h1>
  <p>Name: {name}</p>
  <p>Age: {age}</p>
  <p>Location: {location}</p>
  <p>Hobby: {hobby}</p>
</div>