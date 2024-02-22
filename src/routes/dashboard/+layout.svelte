<script>
  import Sidebar from '$lib/components/Sidebar.svelte';
  import { Button } from '$lib/components/ui/button';
</script>

<div class="grid min-h-screen items-start gap-4 px-4 lg:grid-cols-[280px_1fr]">
  <Sidebar />
  <div class="flex flex-col">
    <header
      class="flex h-14 items-center gap-4 border-b bg-gray-100/40 px-6 dark:bg-gray-800/40 lg:h-[60px]"
    >
      <a class="lg:hidden" href="/">
        <!-- <Package2Icon class="h-6 w-6" /> -->
        <span class="sr-only">Home</span>
      </a>
      <div class="flex-1">
        <nav class="ml-auto flex items-center gap-4">
          <a class="flex items-center gap-3 text-sm font-medium [&]:underline" href="/"> About </a>
          <a class="flex items-center gap-3 text-sm font-medium [&]:underline" href="/">
            Features
          </a>
          <a class="flex items-center gap-3 text-sm font-medium [&]:underline" href="/">
            Pricing
          </a>
          <a class="flex items-center gap-3 text-sm font-medium [&]:underline" href="/">
            Resources
          </a>
          <Button size="sm">Contact</Button>
        </nav>
      </div>
      <Button
        class="h-8 w-8 rounded-full border border-gray-200 dark:border-gray-800"
        size="icon"
        variant="outline"
      >
        <img alt="Avatar" class="rounded-full" height="32" src="/placeholder.svg" width="32" />
        <span class="sr-only">Toggle user menu</span>
      </Button>
    </header>
    <main class="flex flex-1 flex-col gap-4 p-4 md:gap-8 md:p-6">
      <slot />
    </main>
  </div>
</div>
