<script>
  import '../app.css';
  import { page } from '$app/stores';

  let isMenuOpen = false;

  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }

  const navLinks = [
    { label: 'Home', path: '/' },
    { 
      label: 'Personal', 
      path: '/personal', 
      children: [
        { label: 'Projects', path: '/personal/projects' },
        { label: 'Blog', path: '/personal/blog' },
        { label: 'Dev Help', path: '/personal/dev-help' },
      ]
    },
    { 
      label: 'Professional', 
      path: '/professional',
      children: [
        { label: 'Projects', path: '/professional/projects' },
        { label: 'Dev Docs', path: '/professional/dev-docs' },
      ]
    },
    { label: 'About', path: '/about' },
    { label: 'Contact', path: '/contact' },
  ];

  let avatarSrc = "/Logo Icon.favicon 32x29.png";
  let avatarRoute = "/"; 
</script>

<div class="min-h-screen flex flex-col">
  <header class="bg-base-100 shadow-md">
    <div class="navbar container mx-auto">
      <div class="navbar-start">
        <a href={avatarRoute}>
          <div class="avatar">
            <div class="w-8 rounded-full">
              <img src={avatarSrc} alt="Profile" />
            </div>
          </div>
        </a>
      </div>

      <div class="navbar-center hidden lg:flex">
        <ul class="menu menu-horizontal px-1">
          {#each navLinks as link}
            <li class:group={!!link.children} class="relative">
              <a href={link.path} class="flex items-center" class:active={$page.url.pathname === link.path || (link.children && $page.url.pathname.startsWith(link.path))}>
                {link.label}
                {#if link.children}
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-1" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                  </svg>
                {/if}
              </a>
              {#if link.children}
                <ul class="p-2 bg-base-100 bg-opacity-70 rounded-t-none absolute top-full left-0 hidden group-hover:block">
                  {#each link.children as child}
                    <li><a href={child.path} class:active={$page.url.pathname === child.path}>{child.label}</a></li>
                  {/each}
                </ul>
              {/if}
            </li>
          {/each}
        </ul>
      </div>

      <div class="navbar-end lg:hidden">
        <div class="dropdown dropdown-end relative">
          <button class="btn btn-ghost" on:click={toggleMenu}>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h8m-8 6h16" /></svg>
          </button>
          {#if isMenuOpen}
            <ul class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52 absolute right-0 top-full">
              {#each navLinks as link}
                <li>
                  <a href={link.path} class:active={$page.url.pathname === link.path || (link.children && $page.url.pathname.startsWith(link.path))}>
                    {link.label}
                  </a>
                  {#if link.children}
                    <ul class="p-2">
                      {#each link.children as child}
                        <li><a href={child.path} class:active={$page.url.pathname === child.path}>{child.label}</a></li>
                      {/each}
                    </ul>
                  {/if}
                </li>
              {/each}
            </ul>
          {/if}
        </div>
      </div>
    </div>
  </header>

  <main class="flex-grow">
    <div class="container mx-auto p-4">
      <slot />
    </div>
  </main>

  <footer class="footer footer-center p-4 bg-base-300 text-base-content">
    <div class="text-center">
      <div class="flex flex-wrap justify-center gap-8">
        <div class="flex flex-col gap-2">
          <h6 class="footer-title">Navigation</h6>
          <a href="/" class="link link-hover">Home</a>
          <a href="/about" class="link link-hover">About</a>
          <a href="/contact" class="link link-hover">Contact</a>
        </div>
        <div class="flex flex-col gap-2">
          <h6 class="footer-title">Personal</h6>
          <a href="/personal/projects" class="link link-hover">Projects</a>
          <a href="/personal/blog" class="link link-hover">Blog</a>
          <a href="/personal/dev-help" class="link link-hover">Dev Help</a>
        </div>
        <div class="flex flex-col gap-2">
          <h6 class="footer-title">Professional</h6>
          <a href="/professional/projects" class="link link-hover">Projects</a
          >
          <a href="/professional/dev-docs" class="link link-hover">Dev Docs</a
          >
        </div>
        <div class="flex flex-col gap-2">
          <h6 class="footer-title">Legal</h6>
          <a href="/legal" class="link link-hover">License</a>
        </div>
        <div>
          <h6 class="footer-title">Social</h6>
          <a
            href="https://www.tumblr.com/blog/silencewritten"
            class="link link-hover"
          >
          <i class='bx bxl-tumblr bx-sm'></i></a
          >
          <a
            href="https://www.linkedin.com/in/carisa-saenz-videtto-669929173/"
            class="link link-hover"
          >
          <i class='bx bxl-linkedin bx-sm'></i></a
          >
          <a
            href="https://beyondbackend.hashnode.dev/"
            class="link link-hover"
          >
          <i class='bx bx-book-open bx-sm'></i></a
          >
          <a
            href="https://github.com/FizzyMo"
            class="link link-hover"
          >
          <i class='bx bxl-github bx-sm'></i></a
          >
        </div>
      </div>
      <div>
        <p>Copyright © {new Date().getFullYear()} - All right reserved</p>
      </div>
    </div>
  </footer>
</div>