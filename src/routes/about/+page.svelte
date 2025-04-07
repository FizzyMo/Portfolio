<svelte:head>
  <title>About Me</title>
</svelte:head>

<div class="prose max-w-none">
  <h1>About Me</h1>
  
  <div class="flex flex-col md:flex-row gap-8 my-8">
    <div class="md:w-1/3">
      <img src="https://placehold.co/400x500" alt="Profile" class="rounded-lg shadow-lg w-full" />
    </div>
    
    <div class="md:w-2/3">
      <p class="lead">I'm a passionate developer with expertise in web development and a love for creating intuitive, user-friendly applications.</p>
      
      <h2>My Journey</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam in dui mauris. Vivamus hendrerit arcu sed erat molestie vehicula. 
        Sed auctor neque eu tellus rhoncus ut eleifend nibh porttitor. Ut in nulla enim. Phasellus molestie magna non est bibendum non 
        venenatis nisl tempor. Suspendisse dictum feugiat nisl ut dapibus.
      </p>
      
      <h2>Skills</h2>
      <div class="grid grid-cols-2 md:grid-cols-3 gap-4 my-4">
        <div class="badge badge-lg">JavaScript</div>
        <div class="badge badge-lg">Svelte/SvelteKit</div>
        <div class="badge badge-lg">React</div>
        <div class="badge badge-lg">Node.js</div>
        <div class="badge badge-lg">Tailwind CSS</div>
        <div class="badge badge-lg">UI/UX Design</div>
        <div class="badge badge-lg">Git</div>
        <div class="badge badge-lg">Responsive Design</div>
        <div class="badge badge-lg">API Integration</div>
      </div>
      
      <h2>Education</h2>
      <ul>
        <li>Bachelor's Degree in Computer Science - University Name, Year</li>
        <li>Relevant Certification - Organization, Year</li>
      </ul>
    </div>
  </div>
  
  <h2>Work Experience</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <h3 class="text-xl font-bold">Senior Developer - Company Name</h3>
        <p class="text-sm opacity-70">2020 - Present</p>
        <p>
          Responsible for developing and maintaining web applications, collaborating with cross-functional teams, 
          and implementing best practices for code quality and performance.
        </p>
      </div>
    </div>
    
    <div class="timeline-item mt-8">
      <div class="timeline-marker"></div>
      <div class="timeline-content">
        <h3 class="text-xl font-bold">Web Developer - Previous Company</h3>
        <p class="text-sm opacity-70">2017 - 2020</p>
        <p>
          Worked on front-end development using modern JavaScript frameworks, implemented responsive designs, 
          and collaborated with designers to create user-friendly interfaces.
        </p>
      </div>
    </div>
  </div>
</div>

<style>
  .timeline-item {
    position: relative;
    padding-left: 2rem;
  }
  
  .timeline-marker {
    position: absolute;
    top: 0;
    left: 0;
    width: 1rem;
    height: 1rem;
    border-radius: 50%;
    background-color: hsl(var(--p));
  }
  
  .timeline-marker::before {
    content: '';
    position: absolute;
    top: 1rem;
    left: 0.5rem;
    transform: translateX(-50%);
    width: 2px;
    height: calc(100% + 1rem);
    background-color: hsl(var(--p) / 0.3);
  }
  
  .timeline-item:last-child .timeline-marker::before {
    display: none;
  }
</style>