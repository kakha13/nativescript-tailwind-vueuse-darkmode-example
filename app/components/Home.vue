<template>
    <Page>
        <ActionBar>
            <Label text="Home" />
        </ActionBar>

        <GridLayout rows="*, *, auto" columns="*" class="bg-gray-400 dark:bg-slate-900 text-center p-2 w-full">
            <Label row="0" class="text-red-500 dark:text-white text-2xl text-center bg-black" :text="labelOne"></Label>

            <Label row="1" class="text-green-500 dark:text-black text-2xl text-center bg-white" :text="labelTwo"></Label>


            <Button row="2" text="Toggle Theme" @tap="toggleTheme"
                class="bg-slate-800 dark:bg-slate-500 py-2 px-4 text-center text-sm text-white my-4 dark:text-white rounded-lg"></Button>

        </GridLayout>
    </Page>
</template>

<script setup>
import { useDark } from "@nativescript-use/vue";
import { ref, watch } from 'nativescript-vue';

const isDark = useDark();


const toggleTheme = () => {
    isDark.value = !isDark.value;
};

const labelOne = ref("Red");
const labelTwo = ref("Green");

// watch
watch(isDark, (value) => {
    labelOne.value = value ? "White" : "Red";
    labelTwo.value = value ? "Black" : "Green";
});



</script>