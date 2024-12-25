<script>
  import { onNavigate } from "$app/navigation";

  let {children} = $props();

  onNavigate(() => {
    return () => {};
  })
</script>

navigate from another page to <a href="/a">/a</a>, this will register
afterNavigate
<br />
then navigate to <a href="/b">/b</a>
<br>
after navigate should not run but it does
and "after navigate was called" becomes true

<br>
{@render children()}