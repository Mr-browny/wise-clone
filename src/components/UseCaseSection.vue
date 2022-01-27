<template>
    <div class="text-left">
        <div class="grid gap-0 grid-cols-12 sm:grid-cols-2 h-screen" v-for="useCase in useCaseArr" :key="useCase.id">
            <div class="grid place-items-center h-screen px-8" :class="useCase.id % 2 ==0 ? 'order-last': 'order-first'">
                <div class="px-20">
                    <div class="title text-primary">
                        {{ useCase.title }}
                        <span class="dot text-primary-light"></span>
                        <!-- use css ::after to add this part, content: '' -->
                    </div>
                    <div v-for="content in useCase.contentArr" :key="content.id">
                        <div class="subtitle text-primary">
                            {{ content.subtitle }}
                        </div>
                        <div class="content text-text-gray opacity-60">
                            {{ content.description }}
                        </div>
                    </div>
                </div>
            </div>
            <div class="useCase1" :style="{ backgroundImage: 'url(' + useCase.bgImg + ')' }"></div>
        </div>
    </div>
</template>

<style scoped>
    .title{
        font-size: 25px;
        font-weight: bolder;
    }
    .title::after{
        content: '.',

    }
    .subtitle{
        font-size: 17px;
        font-weight: bold;
        padding: 10px 0;
        
    }
    .content{
        color: gray
    }
    .useCase1 {
        /* background-image: url('../assets/img/usecase1.jpg'); */
        /* height: 800px; */
        background-size: cover;
    }
</style>

<script>
export default {
    name: 'UsecaseSection',
    data () {
        return {
            useCaseArr: [
                { 
                    id: 1, title: 'Moving and living abroad just got simpler', bgImg: require('../../src/assets/img/usecase1.jpg'), contentArr: [
                        { id: 0, subtitle: 'Receive your salary, pension, and more.', description: 'Relocate without the stress — and without the multiple bank accounts. Share your details with your employer, pension scheme, family or friends, and get paid like a local.' },
                        { id: 1, subtitle: 'Spend in local currency with your card.', description: 'Avoid the bank appointments, and start spending as soon as you get there. With the Wise debit card, you’ll always get the best possible exchange rate.' },
                        { id: 2, subtitle: 'Move your money between countries.', description: 'Send money to 80 countries, always with a low and transparent fee. With Direct Debits in the UK, Europe, US and Canada, paying your bills and subscriptions across currencies is easier than ever.' },
                    ]
                },
                { 
                    id: 2, title: 'Shopping through overseas online stores', bgImg: require('../../src/assets/img/usecase2.jpg'), contentArr: [
                        { id: 0, subtitle: 'Pay at the real exchange rate.', description: 'Avoid sneaky bank exchange rate markups and high foreign transaction fees. Pay only a low upfront conversion fee, and no annual card fee.' },
                        { id: 1, subtitle: 'Always pay in the local currency.', description: 'If you’re shopping online, always choose to pay in the currency of the country you’re buying from. If you don’t have it in your account, the card will automatically convert to it from the balance that’s cheapest for you. You’ll avoid Dynamic Currency Conversion fees.' },
                        { id: 2, subtitle: 'Pay online securely with instant notifications.', description: 'Authorise payments with 3-D Secure authentication. Receive instant notifications when you spend.' },
                    ]
                },
                { 
                    id: 3, title: 'Receive money from around the world', bgImg: require('../../src/assets/img/usecase3.jpg'), contentArr: [
                        { id: 0, subtitle: 'Get paid like a local.', description: 'UK account number, Euro IBAN, US routing number, and more. All in one account. Receive your salary, invoice payments, pension and profit from shares.' },
                        { id: 1, subtitle: 'Work anywhere and link your account to Amazon, PayPal and more.', description: 'Use your account details to receive and manage your earnings. Invoice like a local and manage your earnings from various online platforms and storefronts.' },
                        { id: 2, subtitle: 'Convert your money in seconds.', description: 'Receive payments from anywhere, and convert them to 54 currencies. You’ll always get the real exchange rate, and the low fees we’re known for.' },
                    ]
                },
                { 
                    id: 4, title: 'Take the stress out of managing property', bgImg: require('../../src/assets/img/usecase4.jpg'), contentArr: [
                        { id: 0, subtitle: 'Save when you buy property abroad.', description: 'Sending and managing money with Wise is on average 6x cheaper than UK banks. And with our tiered pricing for large amounts, you get an even lower fee on any transfers over 100,000 GBP or equivalent in your currency.' },
                        { id: 1, subtitle: 'Pay your bills remotely.', description: 'Hold 54 currencies in one place. Easily manage your mortgage and utility bills across currencies with Direct Debit in the UK, Europe, US and Canada, and pay tradespeople like a local.' },
                        { id: 2, subtitle: 'Receive payments from tenants.', description: 'Get paid in 9 currencies with your own account details. And when the rate is right, convert your money in seconds.' },
                    ]
                }
            ]
        }
    }
}
</script>