<template>
    <div class="px-64">
        <div class="text-center pt-24">
            <div class="text-gray-700"> Coverage </div>
            <div class="text-3xl  mb-10">
                Get these local account details
            </div>
            <div class="text-gray-700"> These are the account details you can share with others to receive money. Anyone can use these to pay you just like they'd pay a local. </div>
        </div>
        <div class="pt-20 pb-10">
            <div class="grid gap-8 grid-cols-1 sm:grid-cols-2 md:grid-cols-3">
                <div class="border border-gray-200 p-8" v-for="i in 12" :key="i">
                    <div class="flex items-center pb-2">
                        <div class="mr-4">
                            <img src="@/assets/icons/icon1.png" alt="icon" width="30" height="30" />
                        </div>
                        <div class="text-2xl text-blue-500"> British pound </div>
                    </div>
                    <div>
                        UK sort code, Account number, and IBAN
                    </div>
                </div>
            </div>
        </div>
        <div class="pt-10">
            <div class="text-center">
                <div class="text-3xl  mb-10">
                Hold and convert money
                </div>
                <div class="text-gray-700"> You can hold and convert money in 54 currencies. It only takes a few seconds to open a new balance in the currency you need. </div>
            </div>
            <div class="pt-20 pb-10">
                <div class="grid gap-1 grid-cols-2 sm:grid-cols-4">
                    <div v-for="i in 56" :key="i">
                        <div class="flex items-center pb-2">
                            <div class="mr-4">
                                <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                            </div>
                            <div class="text-lg"> British pound </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="pt-10">
            <div class="text-center">
                <div class="text-3xl  mb-10">
                Send money to 80 countries
                </div>
                <div class="text-gray-700"> You can use money in your multi-currency account to send to any of the countries on Wise. </div>
            </div>
            <div class="pt-20 pb-10">
                <div class="grid gap-1 grid-cols-2 sm:grid-cols-4">
                    <div v-for="i in 56" :key="i">
                        <div class="flex items-center pb-2">
                            <div class="mr-4">
                                <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                            </div>
                            <div class="text-lg">
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