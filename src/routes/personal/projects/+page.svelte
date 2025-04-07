<svelte:head>
  <title>Personal Projects</title>
</svelte:head>

<div class="max-w-4xl mx-auto">
  <h1 class="text-3xl font-bold mb-6">Personal Projects</h1>
  
  <div class="prose max-w-none mb-8">
    <p>
      These are projects I've built in my free time to explore new technologies, solve personal problems, 
      or just for fun. Each project represents a learning journey and a chance to experiment with different approaches.
    </p>
  </div>
  
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <div class="card bg-base-100 shadow-xl">
      <figure class="relative">
        <video
          src="/walk_through.mp4"
          title="Interactive Narrative"
          autoplay
          loop
          muted
          playsinline
          class="w-lg h-lg object-cover"
        ></video>
      </figure>      <div class="card-body">
        <h2 class="card-title">
          League of Legends Interactive Narrative
          <div class="badge badge-secondary">Personal</div>
        </h2>
        <p>A weather application that provides current conditions and forecasts for any location.</p>
        <div class="flex flex-wrap gap-2 mt-2">
          <div class="badge badge-outline">Python</div>
        </div>
        <div class="card-actions justify-evenly mt-auto">
          
          <a href="https://github.com/FizzyMo/BeyondBackend.Python-Adventure" class="btn btn-sm btn-outline">Source Code</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-xl">
      <figure class="relative">
        <video
          src="/GIF_walk_through.mp4"
          title="Interactive Narrative"
          autoplay
          loop
          muted
          playsinline
          class="w-lg h-lg object-cover"
        ></video>
      </figure>      <div class="card-body">
        <h2 class="card-title">
          GIF Search Application
          <div class="badge badge-secondary">Personal</div>
        </h2>
        <p>A web app for storing and organizing my favorite recipes with search and filtering capabilities.</p>
        <div class="flex flex-wrap gap-2 mt-2">
          <div class="badge badge-outline">HTML</div>
          <div class="badge badge-outline">CSS</div>
          <div class="badge badge-outline">JavaScript</div>
          <div class="badge badge-outline">Bootstrap</div>
          <div class="badge badge-outline">jQuery</div>
          <div class="badge badge-outline">Webpack</div>
          <div class="badge badge-outline">Node.js</div>
          <div class="badge badge-outline">Express</div>
        </div>
        <div class="card-actions justify-end mt-4">
          <a href="https://gif-search-application.vercel.app/" class="btn btn-sm">Live Demo</a>
          <a href="https://github.com/FizzyMo/GIF-Search-Application" class="btn btn-sm btn-outline">Source Code</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-xl">
      <figure><img src="https://placehold.co/600x400" alt="Budget Tracker" /></figure>
      <div class="card-body">
        <h2 class="card-title">
          Budget Tracker
          <div class="badge badge-secondary">Personal</div>
        </h2>
        <p>A simple application to track personal expenses and visualize spending patterns.</p>
        <div class="flex flex-wrap gap-2 mt-2">
          <div class="badge badge-outline">Svelte</div>
          <div class="badge badge-outline">Chart.js</div>
          <div class="badge badge-outline">LocalStorage</div>
        </div>
        <div class="card-actions justify-end mt-4">
          <a href="/" class="btn btn-sm">Live Demo</a>
          <a href="/" class="btn btn-sm btn-outline">Source Code</a>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-xl">
      <figure><img src="https://placehold.co/600x400" alt="Pomodoro Timer" /></figure>
      <div class="card-body">
        <h2 class="card-title">
          Pomodoro Timer
          <div class="badge badge-secondary">Personal</div>
        </h2>
        <p>A productivity timer based on the Pomodoro Technique with customizable work and break intervals.</p>
        <div class="flex flex-wrap gap-2 mt-2">
          <div class="badge badge-outline">JavaScript</div>
          <div class="badge badge-outline">HTML/CSS</div>
          <div class="badge badge-outline">Web Notifications</div>
        </div>
        <div class="card-actions justify-end mt-4">
          <a href="/" class="btn btn-sm">Live Demo</a>
          <a href="/" class="btn btn-sm btn-outline">Source Code</a>
        </div>
      </div>
    </div>
  </div>
</div>