<template>
    <section class="h-screen relative ">
        <!-- <div aria-hidden="true" class="absolute inset-0 grid grid-cols-2 -space-x-52 opacity-40 dark:opacity-20"> -->
        <!-- <div class="blur-[106px] h-56 bg-gradient-to-br from-primary to-purple-400 dark:from-blue-700"></div> -->
        <!-- <div class="blur-[106px] h-32 bg-gradient-to-r from-cyan-400 to-sky-300 dark:to-indigo-600"></div> -->
        <!-- </div> -->
        <div class="text-center flex flex-col justify-center items-center h-screen">
            <h1
                class="font-extrabold text-6xl md:text-9xl [text-wrap:balance] bg-clip-text text-transparent bg-gradient-to-r from-slate-200/60 to-50% to-slate-200 mb-2">
                Summand</h1>
            <h3
                class="font-semibold text-3xl md:text-3xl bg-clip-text text-transparent bg-gradient-to-r from-slate-200/60 to-50% to-slate-200 mb-10">
                New Generation CLI</h3>

            <div class="flex flex-row ">
                <NuxtLink href="https://github.com/summand-dev/summand"
                    class="bg-transparent border-[#587DFF]  border-2 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 flex flex-row items-center justify-center dark:text-white dark:border-[#AEAEAE]">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                        style="fill: rgba(255, 255, 255, 1);transform: ;msFilter:;">
                        <path
                            d="m6.516 14.323-1.49 6.452a.998.998 0 0 0 1.529 1.057L12 18.202l5.445 3.63a1.001 1.001 0 0 0 1.517-1.106l-1.829-6.4 4.536-4.082a1 1 0 0 0-.59-1.74l-5.701-.454-2.467-5.461a.998.998 0 0 0-1.822 0L8.622 8.05l-5.701.453a1 1 0 0 0-.619 1.713l4.214 4.107zm2.853-4.326a.998.998 0 0 0 .832-.586L12 5.43l1.799 3.981a.998.998 0 0 0 .832.586l3.972.315-3.271 2.944c-.284.256-.397.65-.293 1.018l1.253 4.385-3.736-2.491a.995.995 0 0 0-1.109 0l-3.904 2.603 1.05-4.546a1 1 0 0 0-.276-.94l-3.038-2.962 4.09-.326z">
                        </path>
                    </svg>
                    10.2k stars
                </NuxtLink>

                <NuxtLink href="https://docs.summand.dev"
                    class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800 flex flex-row items-center justify-center border-blue-700 border-2">
                    Read docs
                    <svg class="rtl:rotate-180 w-3.5 h-3.5 ms-2 mt-[3px]" aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M1 5h12m0 0L9 1m4 4L9 9" />
                    </svg>

                </NuxtLink>
            </div>
        </div>

    </section>
</template>

