<svelte:head>
  <title>Personal</title>
</svelte:head>

<div class="max-w-4xl mx-auto">
  <h1 class="text-3xl font-bold mb-6">Personal Space</h1>
  
  <div class="prose max-w-none mb-8">
    <p>
      Welcome to my personal space! This is where I share my personal projects, blog posts, and resources 
      that I've found helpful in my development journey.
    </p>
  </div>
  
  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    <a href="/personal/projects" class="card bg-base-100 shadow-xl hover:shadow-2xl transition-shadow">
      <div class="card-body">
        <h2 class="card-title">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2" />
          </svg>
          Personal Projects
        </h2>
        <p>Explore the projects I've built in my free time, including hobby websites, games, and tools.</p>
        <div class="card-actions justify-end">
          <button class="btn btn-primary btn-sm">View Projects</button>
        </div>
      </div>
    </a>
    
    <a href="/personal/blog" class="card bg-base-100 shadow-xl hover:shadow-2xl transition-shadow">
      <div class="card-body">
        <h2 class="card-title">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 20H5a2 2 0 01-2-2V6a2 2 0 012-2h10a2 2 0 012 2v1m2 13a2 2 0 01-2-2V7m2 13a2 2 0 002-2V9a2 2 0 00-2-2h-2m-4-3H9M7 16h6M7 8h6v4H7V8z" />
          </svg>
          Blog
        </h2>
        <p>Read my thoughts on technology, development, and other topics I'm passionate about.</p>
        <div class="card-actions justify-end">
          <button class="btn btn-primary btn-sm">Read Blog</button>
        </div>
      </div>
    </a>
    
    <a href="/personal/dev-help" class="card bg-base-100 shadow-xl hover:shadow-2xl transition-shadow">
      <div class="card-body">
        <h2 class="card-title">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
          </svg>
          Dev Help
        </h2>
        <p>A collection of resources, tips, and solutions to common development problems I've encountered.</p>
        <div class="card-actions justify-end">
          <button class="btn btn-primary btn-sm">Get Help</button>
        </div>
      </div>
    </a>
  </div>
  
  <div class="divider my-12">Recent Activity</div>
  
  <div class="space-y-6">
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <h3 class="card-title">Latest Blog Post: Getting Started with SvelteKit</h3>
        <p class="text-sm opacity-70">Posted 2 weeks ago</p>
        <p>
          In this post, I share my experience with SvelteKit and how it compares to other frameworks I've used.
          Learn about the benefits of Svelte's approach to reactivity and how to get started with your first SvelteKit project.
        </p>
        <div class="card-actions justify-end">
          <a href="/personal/blog" class="btn btn-sm">Read More</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <h3 class="card-title">New Personal Project: Weather Dashboard</h3>
        <p class="text-sm opacity-70">Completed 1 month ago</p>
        <p>
          I built a weather dashboard using Svelte and the OpenWeatherMap API. The app features a clean, 
          responsive design and provides detailed weather information for any location.
        </p>
        <div class="card-actions justify-end">
          <a href="/personal/projects" class="btn btn-sm">View Project</a>
        </div>
      </div>
    </div>
  </div>
</div>