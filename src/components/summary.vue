<template>
    <!-- <div class="flex justify-between">
        <div class="text-green-400">{{ completed }} adet tamamlandÄ±.</div>
        <div class="text-red-400">{{ uncompleted }} adet tamamlanmadÄ±.</div>
    </div> -->
</template>

<script>
import { computed } from "vue";
export default {
    props: {
        todoList: Array,
    },
    setup(props) {
        // const completed = computed(() => props.todoList.filter((i) => i.completed).length);
        // const uncompleted = computed(() => props.todoList.filter((i) => !i.completed).length);

        // return { completed, uncompleted }
    }
}
</script>