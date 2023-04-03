<template>
  <div class="bg-white">
    <main>
      <div
        class="hero bg-gray-900 bg-gradient-to-br from-pink-300 via-red-300/90 to-purple-400 xl:pb-32 pt-6"
      >
      
        <div class="mx-auto max-w-7xl px-8">
          <div class="grid xl:grid-cols-2 xl:gap-8">
            <div
              class="max-w-md px-4 mx-auto sm:max-w-2xl sm:px-6 md:text-center xl:px-0 xl:text-left flex xl:items-center"
            >
              <div class="py-24 z-10">
                <h1
                  class="mb-5 text-4xl font-bold tracking-wide text-white sm:mt-5 sm:text-6xl xl:mt-6"
                >
                  Jeramie Davis.
                </h1>

                <p
                  class="text-base text-white sm:mt-5 sm:text-xl xl:text-lg xl:text-xl"
                >
                  26 year old <span class="font-bold">software developer</span> from British Columbia, Canada.
                </p>
                <p
                  class="text-base text-white sm:text-xl xl:text-lg xl:text-xl"
                >
                  I enjoy creating <span class="font-bold">generative</span> and
                  <span class="font-bold">3D</span> art from time to time.
                </p>

                <div
                  class="flex space-x-6 mt-10 justify-start justify-center xl:justify-start"
                >
                  <a
                    v-for="item in navigation.social"
                    :key="item.name"
                    :href="item.href"
                    class="text-white hover:text-red-200 transition ease-in"
                  >
                    <span class="sr-only">{{ item.name }}</span>
                    <component
                      :is="item.icon"
                      class="h-8 w-8"
                      aria-hidden="true"
                    />
                  </a>
                </div>
              </div>
            </div>

            <div aria-hidden="true" class="hidden md:relative xl:block">
              <svg
                class="absolute left-0 mx-auto mr-8 top-48 2xl:left-16 xl:left-10 md:-left-12"
                width="550"
                height="292"
                fill="none"
                viewBox="0 0 550 292"
              >
                <defs>
                  <pattern
                    id="header-dot-pattern"
                    x="0"
                    y="0"
                    width="20"
                    height="20"
                    patternUnits="userSpaceOnUse"
                  >
                    <rect
                      x="0"
                      y="0"
                      width="4"
                      height="4"
                      class="text-orange-300/50"
                      fill="currentColor"
                    />
                  </pattern>
                </defs>
                <rect
                  width="550"
                  height="292"
                  fill="url(#header-dot-pattern)"
                />
              </svg>

              <img
                src="./assets/saya.png"
                class="overflow-hidden absolute inset-y-0 -mr-6 transition ease-in shadow-lg rounded-md hover:saturate-150 top-16 left-4 w-3/4 h-64"
              />

              <div
                class="overflow-hidden absolute inset-y-0 -mr-6 transition ease-in shadow-lg top-48 xl:left-40 2xl:left-48 w-3/4 h-[250px]"
              >
                <video autoplay loop muted class="rounded-md">
                  <source src="./assets/crumble.mp4" type="video/mp4" />
                </video>
                <div
                  class="absolute inset-0 bg-gradient-to-r from-red-200 to-indigo-600 mix-blend-multiply transition ease-in rounded-md hover:backdrop-hue-rotate-30"
                />
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Gallery -->
      <div
        class="relative py-16 transition-colors duration-200 ease-out bg-black lg:py-24"
      >
        <div class="hidden xl:block">
          <svg
            class="-ml-6 lg:absolute top-16 left-32"
            width="604"
            height="392"
            fill="none"
            viewBox="0 0 604 392"
          >
            <defs>
              <pattern
                id="8228f071-bcee-4ec8-905a-2a059a2cc4fb"
                x="0"
                y="0"
                width="20"
                height="20"
                patternUnits="userSpaceOnUse"
              >
                <rect
                  x="0"
                  y="0"
                  width="4"
                  height="4"
                  class="text-white/5"
                  fill="currentColor"
                />
              </pattern>
            </defs>
            <rect
              width="604"
              height="392"
              fill="url(#8228f071-bcee-4ec8-905a-2a059a2cc4fb)"
            />
          </svg>

          <svg
            class="-mr-6 lg:absolute bottom-16 right-32"
            width="604"
            height="392"
            fill="none"
            viewBox="0 0 604 392"
          >
            <defs>
              <pattern
                id="8228f071-bcee-4ec8-905a-2a059a2cc4fb"
                x="0"
                y="0"
                width="20"
                height="20"
                patternUnits="userSpaceOnUse"
              >
                <rect
                  x="0"
                  y="0"
                  width="4"
                  height="4"
                  class="text-white/5"
                  fill="currentColor"
                />
              </pattern>
            </defs>
            <rect
              width="604"
              height="392"
              fill="url(#8228f071-bcee-4ec8-905a-2a059a2cc4fb)"
            />
          </svg>
        </div>

        <div
          class="relative max-w-md px-4 mx-auto text-center sm:max-w-3xl sm:px-6 lg:px-8 lg:max-w-7xl"
        >
          <h2
            class="text-3xl font-bold tracking-tight text-white sm:text-4xl"
          >
            Artwork
          </h2>

          <section class="overflow-hidden text-gray-700">
            <div class="container mx-auto px-5 py-2 sm:pt-12 lg:pt-24">
              <div class="-m-1 flex flex-wrap md:-m-2">
                <div class="flex flex-wrap">
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/morning in the unknown.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/sunset clouds.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-full p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/monogatari.png"
                      name="Test"
                    />
                  </div>
                </div>
                <div class="flex flex-wrap">
                  <div class="w-1/3 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/fiber optic.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/3 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/alone in a forest.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/3 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/alone in the sea.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/hell baron.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/solar divide.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/moebius.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/upset waters.png"
                      name="Test"
                    />
                  </div>
                </div>
                <div class="flex flex-wrap">
                  <div class="w-full p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/saya.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/downpour.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/2 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/ashes.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/3 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/new life.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/3 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/leaf.png"
                      name="Test"
                    />
                  </div>
                  <div class="w-1/3 p-1 md:p-2">
                    <GalleryImage
                      class="block h-full w-full rounded-lg object-cover object-center"
                      imgSrc="../assets/polaroid.png"
                      name="Test"
                    />
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>
      </div>
    </main>

    <Footer />
  </div>
</template>

<script setup lang="ts">
import { defineComponent, h } from "vue";

import GalleryImage from "./components/GalleryImage.vue";
import Footer from "./components/Footer.vue";

const navigation = {
  social: [
    {
      name: "GitHub",
      href: "https://github.com/EternityX",
      icon: defineComponent({
        render: () =>
          h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
            h("path", {
              "fill-rule": "evenodd",
              d: "M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z",
              "clip-rule": "evenodd",
            }),
          ]),
      }),
    },
    {
      name: "ArtStation",
      href: "https://www.artstation.com/jeramiedavis",
      icon: defineComponent({
        render: () =>
          h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
            h("path", {
              "fill-rule": "evenodd",
              d: "m0 17.723l2.027 3.505h.001a2.424 2.424 0 0 0 2.164 1.333h13.457l-2.792-4.838H0zm24 .025c0-.484-.143-.935-.388-1.314L15.728 2.728a2.424 2.424 0 0 0-2.142-1.289H9.419L21.598 22.54l1.92-3.325c.378-.637.482-.919.482-1.467zm-11.129-3.462L7.428 4.858l-5.444 9.428h10.887z",
              "clip-rule": "evenodd",
            }),
          ]),
      }),
    },
    {
      name: "Deviant Art",
      href: "https://www.deviantart.com/mybrainisdamaged",
      icon: defineComponent({
        render: () =>
          h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
            h("path", {
              d: "M6 6h6l2-4h4v4l-3.5 7H18v5h-6l-2 4H6v-4l3.5-7H6V6Z",
            }),
          ]),
      }),
    },
    {
      name: "Twitter",
      href: "https://twitter.com/etrntycs",
      icon: defineComponent({
        render: () =>
          h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
            h("path", {
              d: "M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84",
            }),
          ]),
      }),
    },
    {
      name: "e-mail",
      href: "mailto:jeramie@pm.me",
      icon: defineComponent({
        render: () =>
          h("svg", { fill: "currentColor", viewBox: "0 0 512 512" }, [
            h("path", {
              "fill-rule": "evenodd",
              d: "M64 112c-8.8 0-16 7.2-16 16v22.1L220.5 291.7c20.7 17 50.4 17 71.1 0L464 150.1V128c0-8.8-7.2-16-16-16H64zM48 212.2V384c0 8.8 7.2 16 16 16H448c8.8 0 16-7.2 16-16V212.2L322 328.8c-38.4 31.5-93.7 31.5-132 0L48 212.2zM0 128C0 92.7 28.7 64 64 64H448c35.3 0 64 28.7 64 64V384c0 35.3-28.7 64-64 64H64c-35.3 0-64-28.7-64-64V128z",
              "clip-rule": "evenodd",
            }),
          ]),
      }),
    },
  ],
};


</script>
