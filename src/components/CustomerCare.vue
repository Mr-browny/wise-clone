<template>
    <div>
        <div class="grid gap-0 grid-cols-12 sm:grid-cols-2 h-screen">
            <div class="useCase1"></div>
            <div class="grid place-items-center text-left h-screen px-8">
                <div class="px-20">
                    <div class="title ">
                        Global support in a range of languages
                        <span class="dot"></span>
                        <!-- use css ::after to add this part, content: '' -->
                    </div>
                    <div class="content">
                        We don’t do complicated, automated systems. We have offices around the world, and we’re here to help you whenever you need it.
                    </div>
                    <button class="mt-4 py-2 px-4 border border-blue-500 hover:border-blue-500 hover:bg-blue-500 hover:text-white">
                        See most frequently asked questions
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .title{
        font-size: 25px;
        color: #1fb6ff;
        font-weight: bolder;
    }
    .title::after{
        content: '.',

    }
    .content{
        color: gray
    }
    .useCase1 {
        background-image: url('../assets/img/callcare.jpg');
        /* height: 800px; */
        background-size: cover;
    }
</style>

<script>
export default {
    name: 'CustomerCare'
}
</script>