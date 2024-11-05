<script>
  export let label = "Input Label"; 
  export let placeholder = "Input text"; 
  export let value = ""; 

  let isFocused = false; 
</script>

<div class="space-y-2">
  <label
    for="input"
    class="block font-medium text-[16px] leading-[16px] text-[#090A0A] mb-[10px] ml-4"
    style="color:black;"
  >
    {label}
  </label>

  <input
    id="input"
    type="text"
    bind:value
    placeholder={placeholder}
    class="w-[327px] h-[48px] border rounded-[8px] border-[#E3E5E5] focus:outline-none focus:border-[#6B4EFF] placeholder:text-[#72777A] m-4"
    on:focus={() => isFocused = true}
    on:blur={() => isFocused = false}
    style="background: #FFFFFF; border-radius: 8px; font-family: 'Inter', sans-serif; font-weight: 400; text-align: left; padding-left: 12px; width: 327px; height: 48px;"
  />
</div>

<style>
  input {
    font-size: 16px;
    line-height: 16px;
    font-weight: 400;
    color: #72777A; 
  }

  input:focus {
    color: #090A0A; 
    border: 2px solid #6B4EFF; 
  }

  input::placeholder {
    color: #72777A; 
  }
</style>

