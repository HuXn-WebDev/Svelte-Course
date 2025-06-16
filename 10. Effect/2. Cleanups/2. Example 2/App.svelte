<script>
  let windowWidth = $state(window.innerWidth);

  $effect(() => {
    const updateWidth = () => {
      windowWidth = window.innerWidth;
    };

    window.addEventListener('resize', updateWidth);
    return () => window.removeEventListener('resize', updateWidth);
  });
</script>

<div>Window width: {windowWidth}px</div>