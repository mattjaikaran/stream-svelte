<script>
  import { Button } from '$lib/components/ui/button';
</script>

<div class="border-r bg-gray-100/40 dark:bg-gray-800/40 lg:block">
  <div class="flex h-full max-h-screen flex-col gap-2">
    <div class="flex h-[60px] items-center border-b px-6">
      <a class="flex items-center gap-2 font-semibold" href="/">
        <!-- <Package2Icon class="h-6 w-6" /> -->
        <span class="">User</span>
      </a>
      <Button class="ml-auto h-8 w-8" size="icon" variant="outline">
        <!-- <BellIcon class="h-4 w-4" /> -->
        <span class="sr-only">Toggle notifications</span>
      </Button>
    </div>
    <nav class="grid items-start px-4 text-sm font-medium">
      <a
        class="flex items-center gap-3 rounded-lg bg-gray-100 px-3 py-2 text-gray-900 transition-all hover:text-gray-900 dark:bg-gray-800 dark:text-gray-50 dark:hover:text-gray-50"
        href="/"
      >
        <!-- <HomeIcon class="h-4 w-4" /> -->
        Home
      </a>
      <a
        class="flex items-center gap-3 rounded-lg px-3 py-2 text-gray-500 transition-all hover:text-gray-900 dark:text-gray-400 dark:hover:text-gray-50"
        href="/"
      >
        <!-- <PackageIcon class="h-4 w-4" />  -->
        Products
      </a>
      <a
        class="flex items-center gap-3 rounded-lg px-3 py-2 text-gray-500 transition-all hover:text-gray-900 dark:text-gray-400 dark:hover:text-gray-50"
        href="/"
      >
        <!-- <UsersIcon class="h-4 w-4" /> -->
        Customers
      </a>
      <a
        class="flex items-center gap-3 rounded-lg px-3 py-2 text-gray-500 transition-all hover:text-gray-900 dark:text-gray-400 dark:hover:text-gray-50"
        href="/"
      >
        <!-- <LineChartIcon class="h-4 w-4" /> -->
        Analytics
      </a>
    </nav>
  </div>
</div>
