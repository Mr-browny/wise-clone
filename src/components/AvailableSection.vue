<template>
    <div class="px-4md:px-24 py-24">
        <div class="flex justify-center items-baseline">
            <div class="text-2xl md:text-4xl font-bold text-primary px-8">Available for you in</div>
            <select class="select-cssd p-4">
                <option value="Nigeria" class="p-4"> Nigeria </option>
                <option value="Nigeria"> Albania </option>
                <option value="Nigeria"> Angola </option>
            </select>
        </div>
        <div class="pt-4 grid gap-8 grid-cols-1 md:grid-cols-4">
            <div class="" v-for="option in availOptions" :key="option.id">
                <div class="flex justify-center">
                    <img :src="option.imgSrc" width="80%" alt="Mobile one" />
                </div>
                <div class="px-2 md:px-0 text-xl font-bold text-center text-primary pb-2 md:pb-4 h-16">
                    {{ option.title }}
                </div>
                <div class="px-2 md:px-0 text-center text-text-gray opacity-60 pb-4">
                     {{ option.content }}
                </div>
                <div v-if="option.link" class="expandable-link  flex justify-center items-baseline  text-primary-light font-bold cursor-pointer" >
                    <div>
                        {{ option.link }}
                    </div>
                    <div class="exapandable-icon pl-1">
                        >
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
</style>

<script>
export default {
    name: 'AvailableSection',
    data (){
        return {
            availOptions: [
                { id: 0, imgSrc: require('../../src/assets/img/mob1.jpg'), title: 'Send money cheaper and easier than old-school banks.', content: 'Send money at the real exchange rate with no hidden fees.', link: 'Send money' },
                { id: 1, imgSrc: require('../../src/assets/img/mob2.jpg'), title: 'Spend abroad without the hidden fees.', content: 'We haven’t reached Algeria with our debit card feature yet.', link: '' },
                { id: 2, imgSrc: require('../../src/assets/img/mob3.jpg'), title: 'Receive payments like a local in 9 currencies.', content: 'Get your own UK account number, Euro IBAN, US routing number, and more.', link: 'See all account details' },
                { id: 3, imgSrc: require('../../src/assets/img/mob4.jpg'), title: 'Convert and hold 54 currencies.', content: 'Holding multiple currencies is completely free, and we use the real exchange rate to convert.', link: 'See all currencies' },
           ]
        }
    }
}
</script>