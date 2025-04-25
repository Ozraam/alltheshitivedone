<script lang="ts">
    import weather from "$lib/assets/appimages/weather.png";
    import connect4 from "$lib/assets/appimages/connect4.png";
    import taquin from "$lib/assets/appimages/taquin.png";
  const apps = [
    {
      icon: "🕹️",
      title: "Connect 4",
      description: "Chalenge the computer to a game of Connect 4 !",
      link: "https://connect4.ozraam.uk",
      image: connect4,
    },
    {
      icon: "🌐",
      title: "Weather",
      description: "Check the weather in your area.",
      link: "https://weather.ozraam.uk",
      image: weather,
    },
    {
      icon: "🧩",
      title: "Taquin",
      description: "Play the classic Taquin game or let the computer solve it.",
      link: "https://taquin.ozraam.uk",
      image: taquin,
    },
  ];
</script>

<section
  class="px-8 pb-16 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 flex-1"
>
  {#each apps as app}
    <div
      class="bg-white rounded-xl shadow-md lg:flex text-center hover:shadow-lg transition h-full overflow-hidden relative"
    >
      <img
        src={app.image}
        alt=""
        class="object-cover lg:w-auto lg:max-w-48 lg:hover:max-w-full transition-all duration-300 ease-in-out"
      />
      <div class="p-6 flex flex-col justify-center flex-1 items-center">
        <div class="text-4xl mb-4">{app.icon}</div>
        <h3 class="text-lg font-semibold">{app.title}</h3>
        <p class="text-sm text-gray-600 mb-4">{app.description}</p>
        <a
          href={app.link}
          target="_blank"
          class="inline-block bg-gray-800 text-white px-4 py-1 rounded hover:bg-gray-700"
        >
          Launch
        </a>
      </div>
    </div>
  {/each}
</section>
