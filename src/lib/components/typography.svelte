<script lang="ts">
  export let variant: 'h1' | 'h2' | 'h3' | 'h4' | 'h5' | 'h6' | 'p' | 'span' | 'a' = 'p';
  export let color:
    | 'primary'
    | 'secondary'
    | 'tertiary'
    | 'success'
    | 'warning'
    | 'danger'
    | 'info'
    | 'light'
    | 'dark' = 'dark';
  export let classname: string = '';
  export let text: string;
  export let href: string = '';
</script>

{#if variant === 'h1'}
  <h1 class="text-4xl font-medium text-{color} {classname}">{text}</h1>
{:else if variant === 'h2'}
  <h2 class="text-3xl font-medium text-{color} {classname}">{text}</h2>
{:else if variant === 'h3'}
  <h3 class="text-2xl font-medium text-{color} {classname}">{text}</h3>
{:else if variant === 'h4'}
  <h4 class="text-xl font-medium text-{color} {classname}">{text}</h4>
{:else if variant === 'h5'}
  <h5 class="text-lg font-medium text-{color} {classname}">{text}</h5>
{:else if variant === 'h6'}
  <h6 class="text-base font-medium text-{color} {classname}">{text}</h6>
{:else if variant === 'p'}
  <p class="text-base text-{color} {classname}">{text}</p>
{:else if variant === 'span'}
  <span class="text-sm text-{color} {classname}">{text}</span>
{:else if variant === 'a'}
  <a class="text-base text-{color} {classname}" {href}>{text}</a>
{/if}
