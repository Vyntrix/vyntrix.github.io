<script lang="ts">
  import { toggleMode } from "mode-watcher";
  import { Button } from "$lib/components/ui/button";
</script>

<Button 
  on:click={toggleMode} 
  variant="outline" 
  size="icon"
>
  <iconify-icon 
    icon="ph:sun-bold" 
    class="rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0">
  </iconify-icon>
  <iconify-icon 
    icon="ph:moon-bold" 
    class="absolute rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100">
  </iconify-icon>
  <span class="sr-only">Toggle theme</span>
</Button>
