<script>
  import { onMount } from 'svelte';

  const title = "Fail. Fail Again. Fail Better.";
  const tagline = "no, seriously";

  onMount(() => {
    document.body.classList.add('admin-page');
    return () => document.body.classList.remove('admin-page');
  });
</script>

<svelte:head>
  <title>{title}</title>
  <meta name="description" content={tagline} />
  <style>
    /* Add any critical styles here temporarily */
    .admin-content {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 8rem;
    }
  </style>
</svelte:head>

<div class="container admin-container">
  <h1>{title}</h1>
  <p>{tagline}</p>

  <section class="admin-content">
    <!-- Users, GOAT, and AI Section -->
    <div class="mb-6">
      <h2>Users</h2>
      <ul class="link-list">
        <li><a href="/manage-users">Manage Users (Auth-n / Auth-z Placeholder)</a></li>
      </ul>
      <h2>GOAT</h2>
      <ul class="link-list">
        <li><a href="https://www.rainharder.com">Rain Harder</a></li>
        <li><a href="https:/games.beer">Games Dot Beer</a></li>
        <li><a href="https:/www.versepedia.org">Versepedia</a></li>
        <li><a href="/hammy">Hammy API</a></li>
      </ul>
      <h2>AI</h2>
      <ul class="link-list">
        <li><a href="/chatgpt">ChatGPT</a></li>
        <li><a href="/copilot">Copilot</a></li>
        <li><a href="/claude">Claude</a></li>
        <li><a href="/supergrok">SuperGrok</a></li>
        <li><a href="/mistral">Mistral</a></li>
      </ul>
    </div>
    <!-- Tools Section -->
    <div class="mb-6">
      <h2>Tools</h2>
      <ul class="link-list">
        <li><a href="https://svelte.dev/">Svelte</a></li>
        <li><a href="https://fastapi.tiangolo.com/">FastAPI</a></li>
        <li><a href="/github">GitHub</a></li>
        <li><a href="/resend">Resend</a></li>
        <li><a href="/plausible">Plausible</a></li>
        <li><a href="/postman">Postman</a></li>
        <li><a href="/vercel">Vercel</a></li>
        <li><a href="/render">Render</a></li>
        <li><a href="/ghost">Ghost</a></li>
        <li><a href="/proton-mail">Proton Mail</a></li>
        <li><a href="/discord">Discord</a></li>
        <li><a href="/godaddy">GoDaddy</a></li>
        <li><a href="/figma">Figma</a></li>
        <li><a href="/google-drive">Google Drive</a></li>
        <li><a href="/slack">Slack</a></li>
        <li><a href="/bluesky">Bluesky</a></li>
        <li><a href="/beekeeper">Beekeeper</a></li>
        <li><a href="/lucid">Lucidchart</a></li>
      </ul>
    </div>
  </section>
</div>
