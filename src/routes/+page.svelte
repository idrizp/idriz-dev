<script lang="ts">
  import Project from "$lib/Project.svelte";
</script>

<svelte:head>
  <title>Idriz's Personal Website</title>
</svelte:head>
<div
  class="px-16 md:px-32 py-5 pt-20 min-h-screen font-serif dark:bg-black dark:text-white tracking-tight"
>
  <p class="text-3xl font-bold font-serif pt-5 text-center">
    Idriz Pelaj's Personal Website:
  </p>
  <p class="text-lg text-center">
    I'm a <span class="text-blue-600 dark:text-blue-300"
      >software developer</span
    >
    and aspiring
    <span class="text-blue-600 dark:text-blue-300">electrical engineer.</span>
  </p>
  <ul
    class="dark:text-blue-400 text-blue-600 text-xl font-bold underline pt-10"
  >
    <li>
      <a href="#about">#about</a>
    </li>
    <li>
      <a href="#work">#work</a>
    </li>
    <li><a href="#education">#education</a></li>
    <li><a href="#info">#info</a></li>
    <li>
      <a href="#projects">#projects</a>
    </li>
    <li>
      <a href="https://idriz.substack.com" target="_blank" rel="noreferrer"
        >#blog</a
      >
    </li>
  </ul>
  <main class="pt-10 gap-y-10 flex-col flex py-20">
    <section id="about">
      <p>
        Hi! I am Idriz. You may notice that this website is <i>quite bland.</i>
      </p>
      <p>
        That's on purpose. I really like these minimalistic
        all-the-info-is-on-the-page style websites.
      </p>
      <p>
        For more of my rants and hot takes on modern web development, check out
        my blog linked above.
      </p>
      <p>
        You'll also find a lot of me experimenting with different things there.
      </p>
      <div class="pt-10">
        <p class="font-bold">
          Current Challenge: <span class="font-normal"
            >52 projects a year, projects done: 2/52</span
          >
        </p>
        <p class="font-bold">
          Learning: <span class="font-normal"
            >Reinforcement Learning w/PyTorch</span
          >
        </p>
      </div>
    </section>
    <section id="work">
      <h2 class="text-2xl font-bold">Work:</h2>
      <ol class="list-disc text-2xl px-5 space-y-3">
        <li>
          <h3>Patrone LLC <span class="font-bold">[2017-2019]</span></h3>
          <p class="text-lg text-blue-600 dark:text-blue-300">
            - Wrote Java code to facilitate cross-server communication.
          </p>
          <p class="text-lg text-blue-600 dark:text-blue-300">
            - Optimized game code to handle over 300 connected players
            simultaneously.
          </p>
        </li>
        <li>
          <h3>LemonGaming LTD <span class="font-bold">[2020-2022]</span></h3>
          <p class="text-lg text-blue-600 dark:text-blue-300">
            - Improved query performance to handle over 200,000 concurrent
            monthly users seamlessly.
          </p>
          <p class="text-lg text-blue-600 dark:text-blue-300">
            - Rewrote core network infrastructure.
          </p>
          <p class="text-lg text-blue-600 dark:text-blue-300">
            - Created staff management system using a Java server with a
            React-based frontend with Tailwind.
          </p>
        </li>
        <li>
          Telara Studios <span class="font-bold">[2022-2022]</span>
          <p class="text-lg text-blue-600 dark:text-blue-300">
            - Wrote code to seamlessly fake player actions to make two separate
            game instances look like one.
          </p>
        </li>
      </ol>
    </section>
    <section id="education">
      <h2 class="text-2xl font-bold">Education:</h2>
      <ol class="list-disc text-lg px-5">
        <li>
          High School: Mehmet Akif School <span class="font-bold"
            >[2019-2022]</span
          >
        </li>
        <li>
          University: Jacobs University Bremen <span class="font-bold"
            >[2022-2025]</span
          >
        </li>
      </ol>
    </section>
    <section id="info">
      <h2 class="text-2xl font-bold">Contact:</h2>
      <ul class="pt-2">
        <li><span class="font-bold">E-Mail:</span> idrizpelaj@hotmail.com</li>
        <li><span class="font-bold">Twitter:</span> idrizp</li>
        <li><span class="font-bold">LinkedIn:</span> idrizpelaj</li>
        <li><span class="font-bold">GitHub:</span>: idrizp</li>
      </ul>
    </section>
    <section id="projects">
      <h2 class="text-2xl font-bold">Projects:</h2>
      <ol class="pt-2 list-disc pl-5 flex gap-y-3 flex-col">
        <Project
          title="commando"
          technologies={["Java", "Maven w/maven modules"]}
        >
          A fully modular command library for perfectionists.
        </Project>
        <Project
          title="cleddit"
          technologies={[
            "Java (server)",
            "Gradle (server)",
            "Spring Boot (server)",
            "NextJS (client)",
            "Tailwind (client)",
          ]}
        >
          <p class="text-blue-600 dark:text-blue-300">A clone of reddit.</p>
        </Project>
        <Project
          title="greenboard"
          technologies={["React Native (client)", "Flask (server)"]}
        >
          <p class="text-blue-600 dark:text-blue-300">
            An app that scans recycling aztec codes and ranks you on a
            leaderboard depending on how much you recycle.
          </p>
        </Project>
        <Project
          title="homefinder"
          technologies={[
            "NextJS (client)",
            "Tailwind (client)",
            "node.js (query processor)",
          ]}
        >
          <p class="text-blue-600 dark:text-blue-300">
            A website that lets you find homes for sale in your area using
            intelligent search with OpenAI(WIP).
          </p>
        </Project>
      </ol>
    </section>
  </main>
</div>
