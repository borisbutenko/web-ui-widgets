<template>
  <div class="min-h-screen flex mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 bg-gray-900">
    <main class="w-full">
      <SliderContainer>
        <SliderSlide
          horizontal-image="https://picsum.photos/seed/test1/1200/500.webp"
          vertical-image="https://picsum.photos/seed/test2/900/1000.webp"
        >
          <div class="flex flex-col gap-2 text-white">
            <p class="text-4xl font-bold ">Trade any in-game items in different games</p>
            <p>Invite friends and get bonuses</p>
            <button class="bg-blue-500 text-white rounded-lg px-4 py-2 text-xl md:w-40 w-full">Try</button>
          </div>
        </SliderSlide>
        <SliderSlide
          horizontal-image="https://picsum.photos/seed/test4/1200/500.webp"
          vertical-image="https://picsum.photos/seed/test5/900/1000.webp"
        >
          <p class="text-4xl text-white"> items in different games</p>
        </SliderSlide>
      </SliderContainer>
      <GameList :games="Cards" header-component="h3" />
    </main>
  </div>
</template>

<script setup lang="ts">
import { GameCard } from "~/components/game/Card.vue"

definePageMeta({
  layout: "home"
})


const Cards: GameCard[] = [
  {
    name: "Apex Legends",
    image: "apex",
    link: "/g/apex"
  },
  {
    name: "GTA 5 Online",
    image: "gta5",
    link: "/g/gta5"
  },
  {
    name: "Genshin Impact",
    image: "genshin",
    link: "/g/genshin"
  },
  {
    name: "Hearthstone",
    image: "hearthstone",
    link: "/g/hearthstone"
  },
  {
    name: "League of Legends",
    image: "lol",
    link: "/g/lol"
  },
  {
    name: "Lineage 2",
    image: "la2",
    link: "/g/la2"
  },
  {
    name: "Minecraft",
    image: "minecraft",
    link: "/g/minecraft"
  },
  {
    name: "Mobile Games",
    image: "mobile",
    link: "/g/mobile-games"
  },
  {
    name: "Path of Exile",
    image: "poe",
    link: "/g/path-of-exile"
  },
  {
    name: "Roblox",
    image: "roblox",
    link: "/g/roblox"
  },
  {
    name: "Rocket League",
    image: "rocket-league",
    link: "/g/rocket-league"
  },
  {
    name: "Rust",
    image: "rust",
    link: "/g/rust"
  },
  {
    name: "Standoff 2",
    image: "standoff2",
    link: "/g/standoff2"
  },
  {
    name: "Steam",
    image: "steam",
    link: "/g/steam"
  },
  {
    name: "Tom Clancy's The Division",
    image: "tom-clansis",
    link: "/g/tc-division"
  },
  {
    name: "Tom Clancy’s Ghost Recon",
    image: "tom-clansis",
    link: "/g/tc-gr"
  },
  {
    name: "Tom Clancy's Rainbow Six",
    image: "tom-clansis",
    link: "/g/tc-rs"
  },
  {
    name: "Valorant",
    image: "valorant",
    link: "/g/valorant"
  },
  {
    name: "Warframe",
    image: "warframe",
    link: "/g/warframe"
  },
  {
    name: "World of Tanks",
    image: "wot",
    link: "/g/wot"
  },
  // {
  //   name: "Overwatch 2",
  //   image: "/game-images/.svg",
  //   link: "/game/2"
  // },
  // {
  //   name: "PlayerUnknown's Battlegrounds (PUBG)",
  //   image: "pubg",
  //   link: "/g/pubg"
  // },
  // {
  //   name: "Uplay",
  //   image: "/game-images/.svg",
  //   link: "/game/2"
  // },
  {
    name: "World of Warcraft",
    image: "wow",
    link: "/g/wow"
  }
]
</script>
