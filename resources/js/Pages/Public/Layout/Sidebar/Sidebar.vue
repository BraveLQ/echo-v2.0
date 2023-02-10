<script setup>
import {Link} from "@inertiajs/vue3";
import {ref} from "vue";

const isOpen = ref(true);
</script>

<template>
    <div class="flex">
        <div
            :class="isOpen ? 'w-20' : 'w-60'"
            class="flex flex-col h-screen p-3 overflow-hidden duration-300 bg-black shadow flex-none"
        >
            <div class="space-y-3">
                <div class="flex items-center justify-between">
                    <img src="/images/png/echo-wb-logo.png" :class="isOpen ? 'hidden': ''" class="h-16 ml-3">
                    <button @click="isOpen = !isOpen" class="mx-auto">
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            stroke="currentColor"
                            class="w-6 h-6 text-white"
                            :class="isOpen ? 'visible': 'hidden'"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                            />
                        </svg>

                        <svg :class="isOpen ? 'hidden': 'visible'" width="24" height="24" viewBox="0 0 35 35" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M4.69429 6.2431C4.5926 6.14141 4.51193 6.02068 4.4569 5.88782C4.40186 5.75495 4.37354 5.61254 4.37354 5.46873C4.37354 5.32491 4.40186 5.18251 4.4569 5.04964C4.51193 4.91677 4.5926 4.79604 4.69429 4.69435C4.79598 4.59266 4.91671 4.51199 5.04958 4.45696C5.18245 4.40192 5.32485 4.3736 5.46867 4.3736C5.61248 4.3736 5.75489 4.40192 5.88776 4.45696C6.02062 4.51199 6.14135 4.59266 6.24304 4.69435L17.4999 15.9534L28.7568 4.69435C28.8585 4.59266 28.9792 4.51199 29.1121 4.45696C29.2449 4.40192 29.3874 4.3736 29.5312 4.3736C29.675 4.3736 29.8174 4.40192 29.9503 4.45696C30.0831 4.51199 30.2038 4.59266 30.3055 4.69435C30.4072 4.79604 30.4879 4.91677 30.5429 5.04964C30.598 5.18251 30.6263 5.32491 30.6263 5.46873C30.6263 5.61254 30.598 5.75495 30.5429 5.88782C30.4879 6.02068 30.4072 6.14141 30.3055 6.2431L19.0465 17.5L30.3055 28.7569C30.4072 28.8585 30.4879 28.9793 30.5429 29.1121C30.598 29.245 30.6263 29.3874 30.6263 29.5312C30.6263 29.675 30.598 29.8174 30.5429 29.9503C30.4879 30.0832 30.4072 30.2039 30.3055 30.3056C30.2038 30.4073 30.0831 30.488 29.9503 30.543C29.8174 30.598 29.675 30.6264 29.5312 30.6264C29.3874 30.6264 29.2449 30.598 29.1121 30.543C28.9792 30.488 28.8585 30.4073 28.7568 30.3056L17.4999 19.0465L6.24304 30.3056C6.14135 30.4073 6.02062 30.488 5.88776 30.543C5.75489 30.598 5.61248 30.6264 5.46867 30.6264C5.32485 30.6264 5.18245 30.598 5.04958 30.543C4.91671 30.488 4.79598 30.4073 4.69429 30.3056C4.5926 30.2039 4.51193 30.0832 4.4569 29.9503C4.40186 29.8174 4.37354 29.675 4.37354 29.5312C4.37354 29.3874 4.40186 29.245 4.4569 29.1121C4.51193 28.9793 4.5926 28.8585 4.69429 28.7569L15.9534 17.5L4.69429 6.2431Z" fill="white"/>
                        </svg>

                    </button>
                </div>
                <div class="flex">
                    <ul class="pt-2 w-full pb-4 space-y-1 text-sm" >
                        <li class="rounded-sm hover:bg-zinc-800 hover:rounded-xl">
                            <a
                                href="#"
                                class="flex items-center p-2 space-x-3 rounded-md"
                            >
                                <img :class="isOpen ? 'mx-auto': ''" src="/icons/i_home.svg">

                                <span :class="isOpen ? 'hidden':'visiable'" class="text-gray-100">Home</span>
                            </a>
                        </li>
                        <li class="rounded-sm hover:bg-zinc-800 hover:rounded-xl ">
                            <a
                                href="#"
                                class="flex items-center p-2 space-x-3 rounded-md"
                            >
                                <img :class="isOpen ? 'mx-auto': ''" src="/icons/i_music.svg">

                                <span :class="isOpen ? 'hidden':'visiable'" class="text-gray-100">Music</span>
                            </a>
                        </li>
                        <li class="rounded-sm hover:bg-zinc-800 hover:rounded-xl ">
                            <a
                                href="#"
                                class="flex items-center p-2 space-x-3 rounded-md"
                            >
                                <img :class="isOpen ? 'mx-auto': ''" src="/icons/i_blog.svg">

                                <span :class="isOpen ? 'hidden':'visiable'" class="text-gray-100">Blog</span>
                            </a>
                        </li>
                        <li class="rounded-sm hover:bg-zinc-800 hover:rounded-xl ">
                            <a
                                href="#"
                                class="flex items-center p-2 space-x-3 rounded-md"
                            >
                                <img :class="isOpen ? 'mx-auto': ''" src="/icons/i_album.svg">

                                <span :class="isOpen ? 'hidden':'visiable'" class="text-gray-100">Album</span>
                            </a>
                        </li>
                        <li class="rounded-sm hover:bg-zinc-800 hover:rounded-xl ">
                            <a
                                href="#"
                                class="flex items-center p-2 space-x-3 rounded-md"
                            >
                                <img :class="isOpen ? 'mx-auto': ''" src="/icons/i_video.svg">

                                <span :class="isOpen ? 'hidden':'visiable'" class="text-gray-100">Video</span>
                            </a>
                        </li>
                        <li class="rounded-sm hover:bg-zinc-800 hover:rounded-xl ">
                            <a
                                href="#"
                                class="flex items-center p-2 space-x-3 rounded-md"
                            >
                                <img :class="isOpen ? 'mx-auto': ''" src="/icons/i_user.svg">

                                <span :class="isOpen ? 'hidden':'visiable'" class="text-gray-100">Singers</span>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="container mx-auto mt-12">

        </div>
    </div>
</template>
