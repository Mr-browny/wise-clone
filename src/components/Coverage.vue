<template>
    <div class="px-8 lg:px-28">
        <div class="text-center pt-24">
            <div class="text-text-gray font-bold"> Coverage </div>
            <div class="text-4xl font-bold text-primary mb-6">
                Get these local account details
            </div>
            <div class="text-text-gray"> These are the account details you can share with others to receive money. Anyone can use these to pay you just like they'd pay a local. </div>
        </div>
        <div class="pt-20 pb-10">
            <div class="grid gap-8 grid-cols-1 sm:grid-cols-2 md:grid-cols-3">
                <div class="border border-text-gray p-8" v-for="i in 12" :key="i">
                    <div class="flex items-center pb-2">
                        <div class="mr-4">
                            <img src="@/assets/icons/icon1.png" alt="icon" width="30" height="30" />
                        </div>
                        <div class="text-lg text-primary"> British pound </div>
                    </div>
                    <div class="font-thin text-text-gray">
                        UK sort code, Account number, and IBAN
                    </div>
                </div>
            </div>
        </div>
        <div class="pt-10">
            <div class="text-center">
                <div class="text-4xl font-bold text-primary mb-6">
                Hold and convert money
                </div>
                <div class="text-text-gray"> You can hold and convert money in 54 currencies. It only takes a few seconds to open a new balance in the currency you need. </div>
            </div>
            <div class="pt-20 pb-10">
                <div class="grid gap-4 grid-cols-1 sm:grid-cols-2 lg:grid-cols-4">
                    <div v-for="i in 56" :key="i">
                        <div class="flex items-center pb-2">
                            <div class="mr-4">
                                <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                            </div>
                            <div class="text-lg text-text-gray"> British pound </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="pt-10">
            <div class="text-center">
                <div class="text-4xl font-bold text-primary mb-6">
                Send money to 80 countries
                </div>
                <div class="text-text-gray"> You can use money in your multi-currency account to send to any of the countries on Wise. </div>
            </div>
            <div class="pt-20 pb-10">
                <div class="grid gap-4 grid-cols-1 sm:grid-cols-2 lg:grid-cols-4">
                    <div v-for="i in 56" :key="i">
                        <div class="flex items-center pb-2">
                            <div class="mr-4">
                                <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                            </div>
                            <div class="text-lg text-text-gray hover:text-primary-light transition ease-in-out hover:ease-in-out">
                                <a href="#" class="underline hover:text-blue-500"> Europe </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Coverage"
}
</script>