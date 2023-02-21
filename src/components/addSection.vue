<template>
    <section class="mt-4">
        <input 
        @keydown.enter="newItem" 
        type="text" 
        placeholder="Todo!" 
        class="w-full p-2 rounded-md bg-gray-700 border outline-none">
    </section>
</template>

<script>
export default {
    props :  {
        AddTodo: Function,
    },
    setup(props){
        const newItem = (event) =>{
            props.AddTodo(event.target.value);
            event.target.value="";
        }
        return { newItem }
    }
}
</script>