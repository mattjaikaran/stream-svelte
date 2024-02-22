<script lang="ts">
  import '../app.pcss';
  import { ModeWatcher } from 'mode-watcher';
  import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />
<ModeWatcher />
<slot />
