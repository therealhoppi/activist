<template>
  <div
    class="flex-1 w-full pt-8 pb-6 bg-light-distinct dark:bg-dark-distinct text-light-text dark:text-dark-text sm:pt-12 sm:pb-10 md:pt-16 md:pb-12 lg:pb-14 lg:pt-20 xl:pt-24 xl:pb-16 2xl:pt-28 2xl:pb-18 space-y-4 sm:space-y-9 xl:space-y-10"
  >
    <div class="flex justify-center">
      <p class="w-10/12 text-2xl font-semibold leading-snug text-center lg:font-bold sm:text-3xl md:text-4xl xl:text-5xl md:max-w-lg xl:max-w-2xl sm:leading-snug md:leading-snug xl:leading-snug">
        {{ $t("landing-header") }}
      </p>
    </div>
    <div class="flex justify-center">
      <p
        class="w-10/12 text-base text-center md:text-lg md:max-w-lg sm:text-xl xl:max-w-2xl xl:text-2xl"
      >
        {{ $t("landing-message") }}
      </p>
    </div>
    <div class="flex justify-center rounded-md">
      <LabeledBtn
        :cta="true"
        :label="`${btnText1}`"
        linkTo="/about"
        fontSize="xl"
      />
    </div>
  </div>
</template>

<script setup>
const localePath = useLocalePath();
const btnText1 = "learn-more";
</script>
