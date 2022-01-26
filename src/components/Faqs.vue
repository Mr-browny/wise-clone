
<template>
    <div class="px-64 bg-gray-200">
        <div class="text-center pt-24">
            <div class="text-gray-300"> Frequently asked questions </div>
            <div class="text-3xl text-white mb-10">
                Let's answer some of your questions
            </div>
        </div>
        <div class="pt-20 pb-10">
            <div class="grid gap-4">
                <div class="p-8 border border-gray-300 bg-white cursor-pointer" v-for="i in 5" :key="i" @click="openAccordion(i)">
                    <div class="title text-xl flex justify-between items-center">
                        <div> What is a multi-currency account and how does it work? </div>
                        <div class="font-bold text-4xl text-blue-500" :class="accordionStatus == i ? 'rotateArrow' : '' "> ^ </div>
                    </div>
                    <div v-if="accordionStatus == i" class="content ">
                        <p>You can hold, receive, send, and spend money using a Wise multi-currency account.
                        <p>You can hold more than 50 currencies, and convert between them at the real exchange rate whenever you need. </p>
                        <p>You can get account details for some currencies to receive money from around the world. </p>
                        <p>You can send money from your account to a bank account whenever you like — we'll charge a fixed fee when you do this, and a conversion fee when you send to a different currency. </p>
                        <p>And, you can spend the currencies in your account around the world with the Wise debit card. Find out if the Wise card is available in your country. </p>
                        <p>Learn more about the multi-currency account in this video </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .rotateArrow {
        transform: rotate(-180deg);
        transition: 0.3s all ease-in-out;
    }
</style>

<script>
export default {
    name: "Faqs",
    data () {
        return {
            accordionStatus: ''
        }
    },
    methods: {
        openAccordion (index) {
            const _ = this;
            _.accordionStatus = _.accordionStatus == index ? '' : index
        }
    }
}
</script>