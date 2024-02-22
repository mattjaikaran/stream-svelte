<script lang="ts">
  import * as DropdownMenu from '$lib/components/ui/dropdown-menu';
  import ThemeToggle from './theme-toggle.svelte';
</script>

<nav
  class="container flex items-center space-x-4 bg-slate-50 p-4 px-8 py-2 text-slate-900 dark:bg-black dark:text-foreground md:py-4 lg:space-x-6"
>
  <div class="mr-auto flex items-center space-x-2">
    <span class="inline-block">Streaming Platform - Svelte</span>
  </div>

  <div class="inline">
    <DropdownMenu.Root>
      <DropdownMenu.Trigger>Menu</DropdownMenu.Trigger>
      <DropdownMenu.Content>
        <DropdownMenu.Group>
          <DropdownMenu.Label>My Account</DropdownMenu.Label>
          <DropdownMenu.Separator />
          <DropdownMenu.Item>Settings</DropdownMenu.Item>
          <DropdownMenu.Item>Logout</DropdownMenu.Item>
        </DropdownMenu.Group>
      </DropdownMenu.Content>
    </DropdownMenu.Root>
  </div>
  <ThemeToggle />
</nav>
