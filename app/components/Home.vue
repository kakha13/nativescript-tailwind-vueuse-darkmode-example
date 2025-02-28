<template>
    <Frame>
        <Page>
            <ActionBar>
                <Label text="Home" />
            </ActionBar>

            <GridLayout rows="*, auto, auto" columns="auto" class="bg-gray-400 dark:bg-slate-900 text-center p-2">
                <Label row="0" class="text-red-300 dark:text-white text-2xl" :text="message"></Label>

                <Label row="1" class="text-red-300 dark:text-white text-2xl" :text="message"></Label>

                <Button row="2" text="Toggle Theme" @tap="toggleTheme"
                    class="bg-gray-600 dark:bg-slate-800 py-2 px-4 text-center text-sm text-white ml-2 dark:text-black"></Button>
            </GridLayout>
        </Page>
    </Frame>
</template>

<script setup>
import { useDark } from "@nativescript-use/vue";
import { ref } from 'nativescript-vue';

const isDark = useDark();


const toggleTheme = () => {
    isDark.value = !isDark.value;
};

const message = ref("Welcome to your Tailwind Vue App");

</script>