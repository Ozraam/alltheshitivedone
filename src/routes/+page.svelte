<script lang="ts">
  import AppGrid from './AppGrid.svelte';

  import HeroPresentation from './HeroPresentation.svelte';

  import Footer from './Footer.svelte';

  import Header from './Header.svelte';
</script>

<div class="min-h-screen bg-gray-50 text-gray-900 flex flex-col">
  <Header />

  <!-- Hero Section -->
  <HeroPresentation />

  <!-- App Grid -->
  <AppGrid />

  <Footer />
</div>
