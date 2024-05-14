<script setup lang="ts">
useHead({
  title: 'LoL Login',
  link: [
    { rel: 'stylespreconnectheet', href: 'https://fonts.googleapis.com' },
    { rel: 'stylespreconnectheet', href: 'https://fonts.gstatic.com' },
    { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap' }
  ]
})
</script>

<template>
  <div class="min-h-screen bg-gray-200 pt-4">
    <main class="m-auto flex max-h-[864px] min-h-[864px] min-w-[1536px] max-w-[1536px] bg-white shadow-xl">
      <div id="login" class="relative flex min-w-[400px] flex-col items-center justify-between bg-white px-[40px]">
        <img class="w-[115px] py-[75px]" src="~/assets/img/riot_games_full.png" />

        <div class="w-11/12">
          <p class="pb-4 text-center text-2xl font-semibold">
            Sign in
          </p>

          <div class="mb-4 w-full rounded bg-gray-100 px-4 py-4 text-[0.7rem] font-semibold text-gray-600">
            <p>USERNAME</p>
          </div>

          <div class="mb-4 w-full rounded bg-gray-100 px-4 py-4 text-[0.7rem] font-semibold text-gray-600">
            <p>PASSWORD</p>
          </div>

          <div class="mt-6 flex w-full justify-between gap-2">
            <span class="grid h-9 w-full place-content-center rounded border bg-blue-700 text-center">
              <img src="https://www.svgrepo.com/show/303114/facebook-3-logo.svg" class="h-5 w-5" />
            </span>
            <span class="grid h-9 w-full place-content-center rounded border bg-white text-center">
              <img src="https://www.svgrepo.com/show/303108/google-icon-logo.svg" class="h-4 w-4" />
            </span>
            <span class="grid h-9 w-full place-content-center rounded border bg-gray-900 text-center">
              <img src="https://upload.wikimedia.org/wikipedia/commons/3/31/Apple_logo_white.svg" class="h-4 w-4" />  
            </span>
            <span class="grid h-9 w-full place-content-center rounded border bg-green-700 text-center">
              <img src="https://upload.wikimedia.org/wikipedia/commons/e/e5/Xbox_Logo.svg" class="h-4 w-4" />
            </span>
          </div>

          <div class="mt-4 flex w-full">
            <span class="mr-2 mt-[2px] inline-block h-[16px] w-[16px] rounded bg-gray-200"> </span>
            <a href="#" class="text-sm font-light">Stay signed in</a>
          </div>

          <div class="h-48 w-full"></div>

          <div class="mx-auto grid h-16 w-16 place-content-center rounded-2xl bg-gray-100">
            <IconsArrowRight class="opacity-50" :size="35" />
          </div>
        </div>



        <div class="flex h-52 w-full flex-col items-center justify-end pb-3 text-[0.7rem]">
          <a href="#" class="pb-1 font-bold uppercase text-gray-700">Can't sign in?</a>
          <a href="#" class="pb-4 font-bold uppercase text-gray-700">Create Account</a>
          <p class="font-bold uppercase text-gray-400">
            This APP is protected by HCAPTCHA and its
          </p>
          <p class="font-bold uppercase text-gray-400">
            <a href="#" class="underline">Privacy Policy</a> and
            <a href="#" class="underline">terms of service</a> apply.
          </p>
        </div>

        <div class="absolute bottom-14 right-10 text-[0.65rem] font-bold text-gray-400">v85.0.1</div>
      </div>

      <div class="w-full bg-[url('https://i.redd.it/qq1e0nz4kwuc1.jpeg')] bg-cover bg-center">
        <div class="flex h-7 items-center justify-end pr-2 text-white">
          <IconsMinus :size="18" class="mr-3" />
          <IconsClose :size="20" />
        </div>
        <div class="flex h-7 items-center justify-between pl-5 pr-12">
          <button class="rounded px-2 py-[2px] text-center text-gray-100 hover:bg-zinc-300/25">
            <IconsTriangleAlert class="mr-1 inline-block fill-yellow-500 stroke-black" :size="23" />
            Gifts
          </button>
          <IconsUserRound :size="40"
            class="mt-10 cursor-pointer rounded-full fill-zinc-300/80 stroke-transparent p-2 hover:bg-zinc-300/10" />
        </div>
      </div>
    </main>


  </div>
</template>

<style scoped>
#login {
  font-family: "Inter", sans-serif;
}
</style>