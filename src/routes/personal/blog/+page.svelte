<svelte:head>
  <title>Blog</title>
</svelte:head>

<div class="max-w-4xl mx-auto">
  <h1 class="text-3xl font-bold mb-6">Blog</h1>
  
  <div class="prose max-w-none mb-8">
    <p>
      Welcome to my blog! Here, I share my thoughts, experiences, and insights on web development, 
      technology trends, and other topics I'm passionate about.
    </p>
  </div>
  
  <div class="flex justify-between items-center mb-6">
    <div class="join">
      <button class="join-item btn btn-sm">All</button>
      <button class="join-item btn btn-sm btn-outline">Development</button>
      <button class="join-item btn btn-sm btn-outline">Design</button>
      <button class="join-item btn btn-sm btn-outline">Technology</button>
    </div>
    
    <div class="form-control">
      <div class="input-group input-group-sm">
        <input type="text" placeholder="Search posts..." class="input input-bordered input-sm" />
        <button class="btn btn-square btn-sm">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" /></svg>
        </button>
      </div>
    </div>
  </div>
  
  <div class="space-y-8">
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <div class="flex justify-between items-start">
          <h2 class="card-title text-2xl">Getting Started with SvelteKit</h2>
          <div class="badge badge-primary">Development</div>
        </div>
        <p class="text-sm opacity-70">Published on June 15, 2025</p>
        <p>
          SvelteKit is a framework for building web applications of all sizes, with a beautiful development experience and flexible 
          filesystem-based routing. In this post, I'll walk you through setting up your first SvelteKit project and explain the key 
          concepts that make it different from other frameworks.
        </p>
        <div class="card-actions justify-end">
          <a href="https://www.w3schools.com/colors/colors_picker.asp" class="btn btn-primary btn-sm">Read More</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <div class="flex justify-between items-start">
          <h2 class="card-title text-2xl">The Power of Tailwind CSS</h2>
          <div class="badge badge-primary">Design</div>
        </div>
        <p class="text-sm opacity-70">Published on May 22, 2025</p>
        <p>
          Tailwind CSS has revolutionized the way I approach styling in web development. In this article, I share my experience 
          transitioning from traditional CSS to utility-first styling, the benefits I've found, and some tips for getting the most 
          out of Tailwind in your projects.
        </p>
        <div class="card-actions justify-end">
          <a href="https://www.w3schools.com/colors/colors_picker.asp" class="btn btn-primary btn-sm">Read More</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <div class="flex justify-between items-start">
          <h2 class="card-title text-2xl">Building a Weather App with the OpenWeatherMap API</h2>
          <div class="badge badge-primary">Development</div>
        </div>
        <p class="text-sm opacity-70">Published on April 10, 2025</p>
        <p>
          In this tutorial, I'll show you how to build a weather dashboard using Svelte and the OpenWeatherMap API. 
          We'll cover fetching and displaying data, handling user input for location search, and creating a responsive 
          design that works well on all devices.
        </p>
        <div class="card-actions justify-end">
          <a href="https://www.w3schools.com/colors/colors_picker.asp" class="btn btn-primary btn-sm">Read More</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <div class="flex justify-between items-start">
          <h2 class="card-title text-2xl">The Future of Web Development: Trends to Watch in 2025</h2>
          <div class="badge badge-primary">Technology</div>
        </div>
        <p class="text-sm opacity-70">Published on March 5, 2025</p>
        <p>
          The web development landscape is constantly evolving. In this post, I explore the emerging trends and technologies 
          that are shaping the future of web development, from AI-assisted coding to new approaches in state management and 
          server-client architecture.
        </p>
        <div class="card-actions justify-end">
          <a href="https://www.w3schools.com/colors/colors_picker.asp" class="btn btn-primary btn-sm">Read More</a>
        </div>
      </div>
    </div>
  </div>
  
  <div class="flex justify-center mt-8">
    <div class="join">
      <button class="join-item btn">1</button>
      <button class="join-item btn btn-active">2</button>
      <button class="join-item btn">3</button>
      <button class="join-item btn">4</button>
    </div>
  </div>
</div>