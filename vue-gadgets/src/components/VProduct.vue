<script setup>
defineProps({
  imgUrl: String,
  title: String,
  price: String,
});
</script>

<template>
  <div class="p-5 bg-slate-100 rounded-xl flex flex-col justify-between gap-2">
    <div>
      <img :src="imgUrl" alt="" class="mb-4" />
      <h3 class="text-xl font-semibold">
        {{ title }}
      </h3>
    </div>
    <div class="flex items-center justify-between gap-2">
      <div>
        <p class="text-slate-500">Цена</p>
        <b class="text-xl">{{ price }} ₽</b>
      </div>
      <div class="flex items-center gap-3">
        <button
          class="rounded-4xl bg-white shadow p-3 cursor-pointer hover:scale-110 transition"
        >
          <a href="" class="flex gap-3 items-center">
            <img src="/like-outline.svg" alt="" />
          </a>
        </button>
        <button
          class="rounded-4xl bg-white shadow p-3 cursor-pointer hover:scale-110 transition"
        >
          <a href="" class="flex gap-3 items-center">
            <img src="/cart-icon.svg" alt="" />
          </a>
        </button>
      </div>
    </div>
  </div>
</template>
