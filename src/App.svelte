<script>
  import InputField from './InputField.svelte';
</script>

<div class="p-[96px] bg-white">
  <!-- Ensure the InputField is being rendered correctly -->
  <InputField 
    label="Input Label" 
    placeholder="Input text" 
    value="" 
  />
</div>

<style>
 
</style>

<svelte:head>
  <link rel="stylesheet" href="https://unpkg.com/tailwindcss@2.2.19/dist/tailwind.min.css" />
</svelte:head>

