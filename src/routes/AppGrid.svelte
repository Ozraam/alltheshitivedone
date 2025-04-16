<script lang="ts">
    const apps = [
        {
            icon: "📱",
            title: "App 1",
            description: "This is a small description for the app.",
            link: ".",
        },
        {
            icon: "📷",
            title: "App 2",
            description: "This is a small description for the app.",
            link: ".",
        },
        {
            icon: "🎮",
            title: "App 3",
            description: "This is a small description for the app.",
            link: ".",
        },
    ];
</script>

<section
    class="px-8 pb-16 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 flex-1"
>
    {#each apps as app}
        <div
            class="bg-white rounded-xl shadow-md md:flex text-center hover:shadow-lg transition h-fit overflow-hidden"
        >
            <img src="https://placehold.co/150" alt="" class="object-cover w-full md:w-auto">
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
