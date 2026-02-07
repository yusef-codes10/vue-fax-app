<script setup>
import { ref } from 'vue'
const array = ref([
  {
    title: 'Lightweight',
    paragraph:
      "I am incredibly small and fast! My core library is only around 30KB, so I won't slow you down.",
  },
  {
    title: 'Approachable',
    paragraph:
      'Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community.',
  },
  {
    title: 'Versatile',
    paragraph:
      "I can handle everything from simple interactive elements to complex single-page applications. I'm great for small projects and large-scale applications alike.",
  },
])

import melody from '@/assets/images/melody.jpeg'
</script>

<template>
  <main>
    <section>
      <h2>
        I'm <span class="highlight">{{ array[0].title }}</span>
      </h2>
      <p>{{ array[0].paragraph }}</p>
    </section>
    <section>
      <h2>
        I'm <span class="highlight">{{ array[1].title }}</span>
      </h2>
      <p>{{ array[1].paragraph }}</p>
    </section>
    <section>
      <h2>
        I'm <span class="highlight">{{ array[2].title }}</span>
      </h2>
      <p>{{ array[2].paragraph }}</p>
    </section>
    <section>
      <!-- Absolute path to /public folder -->
      <img src="/images/melody.jpeg" alt="" />
      <img src="/images/kuromi.jpeg" alt="" />
    </section>

    <section>
      <!-- Relative path to /assets folder -->
      <img src="@/assets/images/melody.jpeg" alt="" />
      <img src="@/assets/images/kuromi.jpeg" alt="" />
    </section>

    <section>
      <!-- Import asset into component -->
      <img v-bind:src="melody" alt="melody" />
    </section>
  </main>
</template>

<style scoped>
main {
  margin-top: 15px;
}

section {
  margin-top: 25px;
}

h2 {
  font-size: 1.3rem;
  color: #34495e;
  margin-bottom: 3px;
}

p {
  font-size: 0.9rem;
  color: #555;
}

img {
  width: 80%;
  height: auto;
  aspect-ratio: 1 / 1;

  margin: 1rem 0;
  border-radius: 50%;
}
</style>
