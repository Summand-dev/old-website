<template>
    <div class="bg-black rounded-t-lg text-center">
        <div class="grid grid-cols-1 gap-4 lg:grid-cols-3 lg:gap-8">
            <div class="h-32 rounded-lg bg-gray-200">
                hi
            </div>
            <div class="h-32 rounded-lg bg-gray-200"> hello </div>
            <div>

                <form class="mt-6 w-full">
                    <label for="UserEmail" class="sr-only"> Email </label>

                    <div class="rounded-md border border-gray-100 p-2 focus-within:ring sm:flex sm:items-center sm:gap-4">
                        <input type="email" id="UserEmail" placeholder="john@rhcp.com"
                            class="w-full border-none focus:border-transparent focus:ring-transparent sm:text-sm" />

                        <button
                            class="mt-1 w-full rounded bg-teal-500 px-6 py-3 text-sm font-bold uppercase tracking-wide text-white transition-none hover:bg-teal-600 sm:mt-0 sm:w-auto sm:shrink-0">
                            Sign Up
                        </button>
                    </div>
                </form>

            </div>
        </div>
        <div>
            <p>Made with 💗</p>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped></style>