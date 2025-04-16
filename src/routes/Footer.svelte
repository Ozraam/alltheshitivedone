<script lang="ts">
  import Header from './Header.svelte';

  const apps = [
    {
      icon: '📱',
      title: 'App 1',
      description: 'This is a small description for the app.',
      link: '.'
    },
    {
      icon: '📷',
      title: 'App 2',
      description: 'This is a small description for the app.',
      link: '.'
    },
    {
      icon: '🎮',
      title: 'App 3',
      description: 'This is a small description for the app.',
      link: '.'
    }
  ];
</script>

<footer class="bg-white text-center p-6 border-t text-sm text-gray-500">
    Let's connect: <a href="https://github.com/Ozraam" class="underline">GitHub</a> | <a href="https://fr.linkedin.com/in/tristan-ardouin-620589223" class="underline">LinkedIn</a>
</footer>

