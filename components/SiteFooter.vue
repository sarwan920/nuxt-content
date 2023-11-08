<script setup>
const links = [
  { name: "Github", href: "https://github.com", icon: "grommet-icons:github" },
  { name: "X", href: "https://x.com", icon: "ri:twitter-x-fill" },
  {
    name: "Facebook",
    href: "https://facebook.com",
    icon: "ic:twotone-facebook",
  },
  { name: "LinkedIn", href: "https://linkedin.com", icon: "bi:linkedin" },
  {
    name: "Instagram",
    href: "https://instagram.com",
    icon: "ri:instagram-fill",
  },
];
</script>
<template>
  <footer class="bg-gray-800">
    <section
      class="mx-auto max-w-7xl px-2 sm:px-4 lg:py-6 text-gray-300 flex flex-row"
    >
      <p class="flex-1 my-auto">&copy; Sarwan Nizamani 2023. All rights reserved</p>
      <div class="flex flex-row justify-center gap-4 mb-4 mt-2">
        <NuxtLink v-for="link in links" :key="link.name" :to="link.href">
          <Icon :name="link.icon" size="1.5rem" class="text-gray-300" />
        </NuxtLink>
      </div>
    </section>
  </footer>
</template>
