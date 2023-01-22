<main>
  <div class="wrapper">
    <nav class="nav">
      <div class="nav-wrapper">
        {#each arr as [item, content]}
          <div class="nav-item-wrapper">
            <div class="nav-item">{item}
              {#if item !== "Fashion"}
              <div class="nav-item-content" hidden>{content}</div>
              {/if}
            </div>
            
          </div>
        {/each}
      </div>
    </nav>
  </div>
</main>



<script>
  const navItems = {
    "Beauty" : "Beauty Content",
    "Fashion": "Fashion Content",
    "Gifts": "Gifts Content",
    "Pets": "Pets Content"
  }

  const arr = Object.entries(navItems);

</script>
