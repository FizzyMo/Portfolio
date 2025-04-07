<svelte:head>
  <title>Professional</title>
</svelte:head>

<div class="max-w-4xl mx-auto">
  <h1 class="text-3xl font-bold mb-6 text-center">Professional Experience</h1>
  
  <div class="prose max-w-none mb-8">
    <!-- Welcome to my professional portfolio. Here you'll find information about my work experience, 
    professional projects, and technical documentation I've created. -->
    <p>
      Fusce ligula erat, rutrum id tortor eget, vestibulum bibendum erat. Aliquam cursus bibendum nunc quis ultricies. Fusce viverra interdum finibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum sit amet augue ut eros vulputate tristique. Praesent molestie suscipit quam, ac convallis felis mollis sit amet. Ut facilisis elementum justo in pellentesque.
    </p>
  </div>
  
  <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-10">
    <a href="/professional/projects" class="card bg-base-100 shadow-xl hover:shadow-2xl transition-shadow">
      <div class="card-body">
        <h2 class="card-title">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
          </svg>
          Professional Projects
        </h2>
        <p>Fusce ligula erat, rutrum id tortor eget, vestibulum bibendum erat. Aliquam cursus bibendum nunc quis ultricies. Fusce viverra interdum finibus.</p>
        <div class="card-actions justify-end">
          <button class="btn btn-primary btn-sm">View Projects</button>
        </div>
      </div>
    </a>
    
    <a href="/professional/dev-docs" class="card bg-base-100 shadow-xl hover:shadow-2xl transition-shadow">
      <div class="card-body">
        <h2 class="card-title">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
          </svg>
          Development Documentation
        </h2>
        <p>Fusce ligula erat, rutrum id tortor eget, vestibulum bibendum erat. Aliquam cursus bibendum nunc quis ultricies. Fusce viverra interdum finibus.</p>
        <div class="card-actions justify-end">
          <button class="btn btn-primary btn-sm">View Documentation</button>
        </div>
      </div>
    </a>
  </div>
  
  <h2 class="text-2xl font-bold mb-4">Work Experience</h2>
  
  <div class="space-y-6">
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <div class="flex flex-col md:flex-row md:justify-between md:items-start">
          <div>
            <h3 class="text-xl font-bold">Senior Web Developer</h3>
            <p class="font-medium">Company Name</p>
          </div>
          <div class="badge badge-lg">2020 - Present</div>
        </div>
        <ul class="mt-4 space-y-2">
          <li class="flex items-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 mt-0.5 text-primary" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
            </svg>
            <span>Led the development of a customer portal that improved client satisfaction by 35%</span>
          </li>
          <li class="flex items-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 mt-0.5 text-primary" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
            </svg>
            <span>Implemented CI/CD pipelines that reduced deployment time by 60%</span>
          </li>
          <li class="flex items-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 mt-0.5 text-primary" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
            </svg>
            <span>Mentored junior developers and conducted code reviews to ensure code quality</span>
          </li>
        </ul>
        <div class="flex flex-wrap gap-2 mt-4">
          <div class="badge badge-outline">React</div>
          <div class="badge badge-outline">Node.js</div>
          <div class="badge badge-outline">AWS</div>
          <div class="badge badge-outline">GraphQL</div>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-md">
      <div class="card-body">
        <div class="flex flex-col md:flex-row md:justify-between md:items-start">
          <div>
            <h3 class="text-xl font-bold">Web Developer</h3>
            <p class="font-medium">Previous Company</p>
          </div>
          <div class="badge badge-lg">2017 - 2020</div>
        </div>
        <ul class="mt-4 space-y-2">
          <li class="flex items-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 mt-0.5 text-primary" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
            </svg>
            <span>Developed responsive web applications for clients across various industries</span>
          </li>
          <li class="flex items-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 mt-0.5 text-primary" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
            </svg>
            <span>Collaborated with designers to implement pixel-perfect UI components</span>
          </li>
          <li class="flex items-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2 mt-0.5 text-primary" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
            </svg>
            <span>Optimized website performance, improving load times by 40%</span>
          </li>
        </ul>
        <div class="flex flex-wrap gap-2 mt-4">
          <div class="badge badge-outline">JavaScript</div>
          <div class="badge badge-outline">Vue.js</div>
          <div class="badge badge-outline">PHP</div>
          <div class="badge badge-outline">MySQL</div>
        </div>
      </div>
    </div>
  </div>
  
  <h2 class="text-2xl font-bold mt-10 mb-4">Skills & Technologies</h2>
  
  <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
    <div class="card bg-base-100 shadow-sm">
      <div class="card-body p-4 text-center">
        <h3 class="font-bold">Frontend</h3>
        <div class="flex flex-wrap justify-center gap-2 mt-2">
          <div class="badge badge-primary">JavaScript</div>
          <div class="badge badge-primary">jQuery</div>
          <div class="badge badge-primary">Svelte</div>
          <div class="badge badge-primary">HTML/CSS</div>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-sm">
      <div class="card-body p-7 text-center">
        <h3 class="font-bold">Backend</h3>
        <div class="flex flex-wrap justify-center gap-2 mt-2">
          <div class="badge badge-primary">Node.js</div>
          <div class="badge badge-primary">Express</div>
          <div class="badge badge-primary">Python</div>
          <div class="badge badge-primary">R</div>
          <div class="badge badge-primary">Java</div>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-sm">
      <div class="card-body p-4 text-center">
        <h3 class="font-bold">Database</h3>
        <div class="flex flex-wrap justify-center gap-2 mt-2">
          <div class="badge badge-primary">MongoDB</div>
          <div class="badge badge-primary">PostgreSQL</div>
          <div class="badge badge-primary">MySQL</div>
          <div class="badge badge-primary">Firebase</div>
          <div class="badge badge-primary">Supabase</div>
        </div>
      </div>
    </div>
    
    <div class="card bg-base-100 shadow-sm">
      <div class="card-body p-4 text-center">
        <h3 class="font-bold">DevOps</h3>
        <div class="flex flex-wrap justify-center gap-2 mt-2">
          <div class="badge badge-primary">Git</div>
        </div>
      </div>
    </div>
  </div>
</div>