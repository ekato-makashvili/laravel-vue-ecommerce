<template>
  <!--
    This example requires updating your template:
 
    ```
    <html class="h-full bg-white">
    <body class="h-full">
    ```
  -->
  <div class="flex min-h-full flex-1 flex-col justify-center px-6 py-12 lg:px-8">
    <div class="sm:mx-auto sm:w-full sm:max-w-sm">
      <img class="mx-auto h-10 w-auto rounded-full"
        src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBwgHBgkIBwgKCgkLDRYPDQwMDRsUFRAWIB0iIiAdHx8kKDQsJCYxJx8fLT0tMTU3Ojo6Iys/RD84QzQ5OjcBCgoKDQwNGg8PGjclHyU3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3N//AABEIAFwAXAMBIgACEQEDEQH/xAAcAAEAAwEAAwEAAAAAAAAAAAAAAQUGBwIDBAj/xAA0EAABAwMCAwYEBAcAAAAAAAABAAIDBAUREiEGMUEUIlFhcaETI4GxBzJCkRUWUlNikvD/xAAZAQEBAQEBAQAAAAAAAAAAAAAAAwEEAgX/xAAgEQADAAICAQUAAAAAAAAAAAAAAQIDERJBBBMhMTJx/9oADAMBAAIRAxEAPwDhqIiAIiIAiIgCIiAIiIAiIgCIiAIvdS0s1XPHBTRmSWQ4axvMrTw8AXZ7AZJaSJ39Lnkn2CpGK7+q2Vx4MmX6TsySnBWsHA9TG/FXX00TfENe4/YLccE8AWdkBrK3Fxc44jEjcMaBzOnqem685YrFPKkUnxMzemtHHY4pJHaY2Oe7waMlTPBNTv0VET4n4zpe0tOPQr9HxWultzSyipooIG7/ACmBunxz4j7LhXGs8tZxHW1L4nsidJoiLmkAtaMAjIHPGfqo48nqLaRvkeMsMputtlCiIqHKEREAREQGj4Xq/wCG2+7XCJrTUxRsjicf063EE+w/ZU5uFYZzP2uf4pOdYkOV401W6CCpgAyydga4Z5EOBB9vdXlm4adVUoq6wmOJw1NGQ3u+JJ5BVTqkpXRflVzMT0fbZuN6iHENyY+dnIPj/N9RyPsuv2a50NHZqaa4R9la/ZrZGlh3ydx0PksZ+HnCloFVJdNXanQP0wBxyxrxuXDbcjbHMLZXo04bC2WASgvyGlodjbnv6romatccnujrWXLGNu3+EXPi21SU0kFG8tLhp1mJxHsFTU09r+E4ztlkZ1c4YYPUlVPGd2o7NS09RHRNdLK8tDRhmwGc8v8AsrmN6u8t1mDntLI28ma9W/itqseGeE/J8a/UzZedfCNLx3LwmYgLLAO3ucMvp3/KaOuehPp9ViERcTe3ssloIiLDQiIgJXSOIIX1Vion0gJi/MQ3lgbD9se65utrwVxPT0kTbbdnFsAdmGf+3no7y8+n2thpJtPsvgpJtPstbPcLja7DpNbDQUMTi58oh1yOLjyGds9OXRfN/OlPSTO0Ulyrax2Bqq3hp8gGjOPRWP4i0Mr7JTVtuAdDTzCWQx7jBHdf6Ag/7Kgraukrux3CO4Qw3MxNa5xfgOOh2trgMaN9gQf1Kt3UvSNyt70UN/u9ffKp1TWNIbH3Gsa06YvL19VWNje44axxOM7Dot3V3K3VLqqLt8Yhm7QJMOwC5zogDjrjvYP+JXtorla4aqSeKsjhGhsbYzLsyON7gA0+Ywccznqo8Nv3ZzU9HPtDt+67u7HbkvFbmruVI6nrGtrIiJIpQ9vxB8x3Z4w317wP1BWHK8VKRkvZCIi8noIiIApUIgNTwjxbLZZH09drqbbLC+J0Gx056jPn08ysvlQi1ttaNbbJyUyVCLDCclQiIAiIgCIiAIiIAiIgCIiAIiIAiIgP/9k="
        alt="Your Company" />
      <h2 class="mt-10 text-center text-2xl/9 font-bold tracking-tight text-gray-900">Request new password</h2>
    </div>

    <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">
      <form class="space-y-6" action="#" method="POST">
        <div>
          <label for="email" class="block text-sm/6 font-medium text-gray-900">Email address</label>
          <div class="mt-2">
            <input type="email" name="email" id="email" autocomplete="email" required=""
              class="block w-full rounded-md bg-white px-3 py-1.5 text-base text-gray-900 outline-1 -outline-offset-1 outline-gray-300 placeholder:text-gray-400 focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-600 sm:text-sm/6" />
          </div>
        </div>

        <div class="flex items-center justify-between">
          <div class="text-sm">
            <router-link :to="{ name: 'login' }" class="font-semibold text-indigo-600 hover:text-indigo-500">Go to login page</router-link>
          </div>
        </div>

        <div>
          <button type="submit"
            class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm/6 font-semibold text-white shadow-xs hover:bg-indigo-500 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Submit
          </button>
        </div>
      </form>
    </div>
  </div>
</template>