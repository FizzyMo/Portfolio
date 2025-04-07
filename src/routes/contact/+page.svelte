<script>
  let formData = {
    name: '',
    email: '',
    subject: '',
    message: ''
  };
  
  let submitted = false;
  let error = false;
  
  function handleSubmit() {
    // In a real application, you would send this data to your backend
    console.log('Form submitted:', formData);
    
    // Simulate form submission
    if (formData.name && formData.email && formData.message) {
      submitted = true;
      error = false;
    } else {
      error = true;
    }
  }
</script>

<svelte:head>
  <title>Contact Me</title>
</svelte:head>

<div class="max-w-3xl mx-auto">
  <h1 class="text-3xl font-bold mb-6">Contact Me</h1>
  
  {#if submitted}
    <div class="alert alert-success mb-6">
      <svg xmlns="http://www.w3.org/2000/svg" class="stroke-current shrink-0 h-6 w-6" fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
      <span>Thank you for your message! I'll get back to you soon.</span>
    </div>
  {:else}
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      <div>
        <p class="mb-4">
          I'd love to hear from you! Whether you have a question, a project idea, or just want to say hello, 
          feel free to reach out using the form or through my social media channels.
        </p>
        
        <div class="card bg-base-200 shadow-sm p-4 mb-4">
          <h3 class="font-bold mb-2">Email</h3>
          <p>contact@example.com</p>
        </div>
        
        <div class="card bg-base-200 shadow-sm p-4 mb-4">
          <h3 class="font-bold mb-2">Location</h3>
          <p>City, Country</p>
        </div>
        
        <div class="flex gap-4 mt-6">
          <a href="/" class="btn btn-circle btn-outline">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"></path></svg>
          </a>
          <a href="/" class="btn btn-circle btn-outline">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"></path></svg>
          </a>
        </div>
      </div>
      
      <div>
        {#if error}
          <div class="alert alert-error mb-6">
            <svg xmlns="http://www.w3.org/2000/svg" class="stroke-current shrink-0 h-6 w-6" fill="none" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 14l2-2m0 0l2-2m-2 2l-2-2m2 2l2 2m7-2a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
            <span>Please fill out all required fields.</span>
          </div>
        {/if}
        
        
        <form on:submit|preventDefault={handleSubmit} class="space-y-4">
          <div class="form-control">
            <label for="name" class="label">
              <span class="label-text">Name*</span>
            </label>
            <input 
              type="text" 
              id="name" 
              bind:value={formData.name} 
              class="input input-bordered w-full" 
              required
            />
          </div>
          
          <div class="form-control">
            <label for="email" class="label">
              <span class="label-text">Email*</span>
            </label>
            <input 
              type="email" 
              id="email" 
              bind:value={formData.email} 
              class="input input-bordered w-full" 
              required
            />
          </div>
          
          <div class="form-control">
            <label for="subject" class="label">
              <span class="label-text">Subject</span>
            </label>
            <input 
              type="text" 
              id="subject" 
              bind:value={formData.subject} 
              class="input input-bordered w-full"
            />
          </div>
          
          <div class="form-control">
            <label for="message" class="label">
              <span class="label-text">Message*</span>
            </label>
            <textarea 
              id="message" 
              bind:value={formData.message} 
              class="textarea textarea-bordered h-32" 
              required
            ></textarea>
          </div>
          
          <button type="submit" class="btn btn-primary">Send Message</button>
        </form>
      </div>
    </div>
  {/if}
  
</div>