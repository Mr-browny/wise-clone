<template>
    <div class="px-28 bg-gray">
        <div class="text-center pt-24">
            <div class="text-text-gray"> Security </div>
            <div class="text-primary text-4xl mb-6">
                Protecting you and your money
            </div>
            <div class="text-text-gray"> Every month, our customers trust us to move over £6 billion of their money. Here are some of the important ways we protect them.</div>
        </div>
        <div class="pt-20 pb-5">
            <div class="grid gap-4 grid-cols-1 sm:grid-cols-2">
                <div class="flex justify-between bg-white p-10" v-for="security in securityOptions" :key="security.id">
                    <div class="pr-8 text-center grid content-center justify-center">
                        <img :src="security.imgSrc" alt="icon" width="100" height="100" />
                    </div>
                    <div class="text-left">
                        <div class="text-primary font-bold text-lg"> {{ security.title }} </div>
                        <div class="text-text-gray pt-4">
                            {{ security.content }}
                            <a href="#"> here </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="text-center text-text-gray pt-5 pb-10">
            Online scams are on the rise. 
            <a href="#" class="underline text-primary-light"> Learn how to stay safe </a>
        </div>
    </div>
</template>

<script>
export default {
    name: "Security",
    data (){
        return {
            securityOptions: [
                { id: 0, imgSrc: require('../../src/assets/icons/icon1.png'), title: 'Safeguarded with leading banks', content: 'We hold your money with established financial institutions, so it’s separate from our own accounts and in our normal course of business not accessible to our partners. Read more' },
                { id: 1, imgSrc: require('../../src/assets/icons/icon2.png'), title: 'Regulated around the world', content: 'We’re regulated by authorities around the world. This includes the FCA in the UK and FinCEN in the US.' },
                { id: 2, imgSrc: require('../../src/assets/icons/icon3.png'), title: 'Audited regularly', content: 'We make sure your money’s secure, and that Wise is financially stable. As we’re not a bank, your money isn’t FSCS protected — instead we safeguard it.' },
                { id: 3, imgSrc: require('../../src/assets/icons/icon4.png'), title: 'Extra-secure transactions', content: 'We use 2-factor authentication to protect your account and transactions. That means you — and only you — can get to your money.' },
                { id: 4, imgSrc: require('../../src/assets/icons/icon5.png'), title: 'Data protection', content: 'We’re committed to keeping your personal data safe, and we’re transparent in how we collect, process, and store it.' },
                { id: 5, imgSrc: require('../../src/assets/icons/icon6.png'), title: 'Dedicated anti-fraud team', content: 'We work round the clock to keep your account and money protected from even the most sophisticated fraud.' },
           ]
        }
    }
}
</script>