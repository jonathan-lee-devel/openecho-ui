<script lang="ts">
  import '../app.css';

  import {ModeWatcher} from 'mode-watcher';
  import DarkModeToggle from '$lib/components/DarkModeToggle.svelte';
  import { Button } from '$lib/components/ui/button';
</script>

<ModeWatcher />
<nav class="bg-white border-gray-200 dark:bg-gray-900">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
    <a class="flex items-center space-x-3 rtl:space-x-reverse" href="https://flowbite.com/">
      <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">OpenEcho</span>
    </a>
    <div class="flex md:order-2 space-x-3 md:space-x-0 rtl:space-x-reverse">
      <Button variant="outline">Get Started</Button>
      <div class="mx-3 px-3">
        <DarkModeToggle />
      </div>
    </div>
  </div>
</nav>
<slot />
