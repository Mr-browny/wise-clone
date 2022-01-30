<template>
    <div class="linear_gradient text-white py-24 px-8 sm:24 lg:px-54">
        <!-- you will be using a linear gradient here.. -->
        <div class="text-center">
            <div class="text-lg"> Getting started</div>
            <div class="text-4xl font-bold pt-8 pb-8 md:pb-24">
                Get set up and start spending with your card in <br> minutes.
            </div>
            <div class="grid gap-5 grid-cols-1 md:grid-cols-4">
                <div class="md:hidden text-center">
                    <div>
                        {{ firstGetStartedArr.content }}
                    </div>
                </div>
                <div class="hidden md:block" v-for="getStarted in getStartedArr" :key="getStarted.id">
                    <div class="font-bold text-2xl mb-8"> {{ getStarted.title }} </div>
                    <!-- Add an image here and use vif to toggle it -->
                    <div v-if="!getStarted.title" class="flex justify-center" style="margin-top: -48px;">
                        <img src="@/assets/icons/good.png" width="58" height="58" class="mb-4" />
                    </div>
                    <div class="">
                        {{ getStarted.content }}
                    </div>
                </div>
            </div>
            <button class="text-2xl my-12 py-4 px-8 border border-white hover:border-primary-light hover:bg-primary-light transition ease-in-out hover:ease-in-out text-white"> Get an account in minutes </button>
        </div>
    </div>
</template>

<style scoped>
    .linear_gradient {
            background: linear-gradient( 252.32deg,#485dc7 0%,#37517e 100%),linear-gradient(0deg,#475cc7,#475cc7);
    }
</style>

<script>
export default {
    name: 'GetStarted',
    computed: {
        firstGetStartedArr () {
            const _ = this
            return _.getStartedArr[0]
        }
    },
    data () {
        return {
            getStartedArr: [
                {id: 0, title: 'Register in minutes', content: 'Sign up online, or in our app with an email address, or a Google, Facebook or Apple account.' },
                {id: 1, title: 'Verify your identity', content: 'All you need to receive money or order a card is your government ID.' },
                {id: 2, title: 'Top up your account', content: 'You can add money using your bank account, Apple Pay, credit/debit card.' },
                {id: 3, title: '', content: 'Share your account details to get paid, or spend around the world with your debit card.' },
            ]
        }
    }
}
</script>