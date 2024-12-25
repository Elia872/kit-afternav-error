<script>
  import { afterNavigate } from "$app/navigation";

  afterNavigate(() => {
    const el = document.querySelector('.after-nav-target');

    console.log("after nav")

    if (el) {
      el.innerText = true;
    }
  })
</script>
<div>/a</div>
