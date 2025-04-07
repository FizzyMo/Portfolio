<script>
  // Home page component
</script>

<svelte:head>
  <title>Beyond Backend</title>
</svelte:head>
<section class="hero min-h-[50vh]">
  <div class="hero text-center">
    <div class="max-w">
      <h1 class="text-[200px] font-bold p-2 tracking-wide">
        Carisa Saenz-Videtto
      </h1>
      <p>"Coding is the best and largest puzzle"</p>
    </div>
  </div>
</section>

<section class="py-10">
  <h2 class="text-3xl font-bold text-center mb-8">Featured Projects</h2>
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
    <div class="card bg-base-100 shadow-xl">
        <figure class="relative">
          <video
            src="/dataset.gen.mp4"
            title="Dataset Generation"
            autoplay
            loop
            muted
            playsinline
            class="w-lg h-lg object-cover"
          ></video>
        </figure>
        <div class="card-body">
          <h2 class="card-title font-bold">Dataset Generation</h2>
          <p>A brief description of the project and the technologies used.</p>
          <div class="card-actions justify-end">
            <a
              href="https://github.com/FizzyMo/BeyondBackend.Large-Dataset-Generation"
              class="btn btn-primary btn-sm">View Details</a
            >
          </div>
        </div>
    </div>

    <div class="card bg-base-100 shadow-xl">
      <figure class="relative">
        <video
          src="/console.data_analysis.mp4"
          title="Data Analysis"
          autoplay
          loop
          muted
          playsinline
          class="w-lg h-lg object-cover"
        ></video>
      </figure>
      <div class="card-body">
        <h2 class="card-title font-bold">Data Analysis and Interpretation</h2>
        <p>A brief description of the project and the technologies used.</p>
        <div class="card-actions justify-end">
          <a
            href="https://github.com/FizzyMo/BeyondBackend.Data-Analysis-and-Interpretation"
            class="btn btn-primary btn-sm">View Details</a
          >
        </div>
      </div>
    </div>

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
      </figure>
      <div class="card-body">
        <h2 class="card-title font-bold">
          League of Legends Interactive Narrative
        </h2>
        <p>A brief description of the project and the technologies used.</p>
        <div class="card-actions justify-end">
          <a
            href="https://github.com/FizzyMo/BeyondBackend.Python-Adventure"
            class="btn btn-primary btn-sm">View Details</a
          >
        </div>
      </div>
    </div>
  </div>
</section>
