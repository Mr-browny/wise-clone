<template>
    <div>
        <div class="grid gap-0 grid-cols-1 lg:grid-cols-2 h-screen">
            <div class="useCase1"></div>
            <div class="grid place-items-center text-left h-screen px-8">
                <div class="px-2 text-center lg:text-left lg:px-20">
                    <div class="text-primary-light text-4xl">
                        Global support in a range of languages
                        <span class="dot"></span>
                        <!-- use css ::after to add this part, content: '' -->
                    </div>
                    <div class="text-text-gray mt-6">
                        We don’t do complicated, automated systems. We have offices around the world, and we’re here to help you whenever you need it.
                    </div>
                    <button class="text-2xl my-12 py-4 px-8 border border-primary-light hover:border-primary-light hover:bg-primary-light transition hover:transition ease-in-out hover:ease-in-out text-primary-light hover:text-white">
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