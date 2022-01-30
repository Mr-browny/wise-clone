<template>
    <div class="bg-landing-page-light px-4 lg:px-12">
        <!-- <div class="skewed_bg h-full bg-landing-page-dark"></div> -->
        <div class="flex justify-between py-10">
            <div class="flex justify-start items-baseline w-6/12">
                <img src="https://wise.com/public-resources/assets/logos/wise/brand_logo_inverse.svg" alt="Wise" class="pr-4">
                <div class="hidden lg:flex text-white font-bold">
                    <div class="text-2xl pr-4 text-primary-light cursor-pointer"> Personal </div>
                    <div class="w-px h-8 bg-text-gray"></div>
                    <div class="text-2xl pl-4 cursor-pointer hover:text-primary-light"> Business </div>
                </div>
            </div>
            <div class="hidden lg:flex w-3/4 justify-evenly items-baseline  font-bold text-xl text-white">
                <div class="relative">
                    <div class="link-title text-sm cursor-pointer hover:text-primary-light transition ease-in-out hover:transition">
                        Money transfer
                        <span class="text-xs"> &#9660; </span>
                    </div>
                    <div class="card">
                        <div class="pointer"></div>
                        <div class="header cursor-pointer">
                            <div>
                                <img src="https://daw291njkc3ao.cloudfront.net/conversion/navigation/send-money.svg" alt="icon" width="" height="" />
                            </div>
                            <div class="flex text-primary-dark py-4">
                               Send Money
                                <span class="ml-2 caret-right text-primary-light"> > </span>
                            </div>
                            <div class="text-text-gray opacity-50 text-sm">
                                Make a one off-payment. You'll get the real exchange rage with the low fee we're known for.
                            </div>
                        </div>
                        <div class="content">
                            <div class="divider"></div>
                            <ul class="list grid gap-4">
                                <li v-for="i in moneyTransferArr" :key="i" class="text-primary-dark cursor-pointer">
                                    <div class="flex">
                                        {{ i }}
                                        <span class="ml-2 caret-right text-primary-light"> > </span>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="relative">
                    <div class="link-title text-sm cursor-pointer hover:text-primary-light transition ease-in-out hover:transition">
                        Multi-currency account
                        <span class="text-xs"> &#9660; </span>
                    </div>
                    <div class="card">
                        <div class="pointer"></div>
                        <div class="header cursor-pointer">
                            <div>
                                <img src="https://wise.com/public-resources/assets/public-navigation/multi_currency_account_v2.svg" alt="icon" width="" height="" />
                            </div>
                            <div class="flex text-primary-dark py-4">
                               Multi-currency account
                                <span class="ml-2 caret-right text-primary-light"> > </span>
                            </div>
                            <div class="text-text-gray opacity-50 text-sm">
                                Manage your money accross 50+
                                currencies. Send at the real exchange rate, and spend with
                                a Wise debit card.
                            </div>
                        </div>
                        <div class="content">
                            <div class="divider"></div>
                            <ul class="list grid gap-4">
                                <li v-for="i in multiCurrencyAccountArr" :key="i" class="text-primary-dark cursor-pointer">
                                    <div class="flex">
                                        {{ i }}
                                        <span class="ml-2 caret-right text-primary-light"> > </span>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer"> Help </div>
                <div class="relative">
                    <div class="link-title text-sm cursor-pointer hover:text-primary-light transition ease-in-out hover:transition">
                        &#127760; EN
                        <span class="text-xs"> &#9660; </span>
                    </div>
                    <div class="card">
                        <div class="pointer"></div>
                        <div class="header">
                            <div class="text-primary text-2xl"> Hello World </div>
                        </div>
                        <div class="content">
                            <div class="divider"></div>
                            <ul class="list grid grid-cols-2 gap-4">
                                <li v-for="i in 16" :key="i" class="text-text-gray hover:text-primary-light cursor-pointer transition hover:transition ease-in-out"> Deutsh </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="cursor-pointer"> Log in</div>
            </div>
            <div class="grid items-center">
                <div class="cursor-pointer border border-solid border-primary-light text-primary-light transition ease-in-out hover:transition hover:ease-in-out hover:bg-primary-light hover:text-white px-4 py-2 items-baseline"> Register </div>
            </div>
        </div>
        <div class="pt-10 sm:px-24 pb-20 grid grid-cols-1 lg:grid-cols-2">
            <div class="flex flex-col justify-between">
                <div class="lg:hidden flex justify-center mt-4 mb-8">
                    <div class="video_pulse bg-primary-light text-white w-28 h-28 rounded-full grid items-center text-center text-5xl">
                        <div class="text-white"> &#9660; </div>
                    </div>
                </div>
                <div class="text-2xl md:text-4xl mb-12 md:mb-0 text-white font-bold text-center lg:text-left"> The cheap, fast wasy to send money <br> abroad. </div>
                <div class="hidden lg:flex">
                    <div class="video_pulse bg-primary-light text-white w-28 h-28 rounded-full grid items-center text-center text-5xl">
                        <div class="text-white"> &#9660; </div>
                    </div>
                    <div class="text-primary-light grid items-center ml-8">
                        <div class="cursor-pointer transition ease-in-out hover:opacity-90 text-xl"> See how it works </div>
                    </div>
                </div>
                <div class="hidden lg:grid grid-cols-2">
                    <div>
                        <h3 class="text-white"> Over 12 million customers </h3>
                        <div class="expandable-link  flex items-baseline  text-primary-light font-bold cursor-pointer transition ease-in-out hover:opacity-90">
                            <div>
                                Read on Trustpilot
                            </div>
                            <div class="exapandable-icon pl-1">
                                >
                            </div>
                        </div>
                    </div>
                    <div>
                        <h3 class="text-white"> FCA regulated </h3>
                        <div class="expandable-link  flex items-baseline  text-primary-light font-bold cursor-pointer transition ease-in-out hover:opacity-90">
                            <div>
                                Learn more
                            </div>
                            <div class="exapandable-icon pl-1">
                                >
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="lg:pl-30 mt-24 lg:mt-0">
                <div class="flex">
                    <div class="bg-white py-2 w-full">
                        <div class="text-lg px-4 text-text-gray opacity-60"> You send </div>
                        <input type="tel" value="1,000" class="px-4 py-2 outline outline-none text-2xl w-full" />
                    </div>
                    <div class="bg-landing-page-dark cursor-pointer flex items-center justify-center w-6/12 hover:border hover:border-white hover:border-2">
                        <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                        <div class="px-4 text-3xl font-bold text-white"> GBP </div>
                        <div class="text-primary-light">  &#9660; </div>
                    </div>
                </div>
                <div class="flex items-center  my-3 pl-12">
                    <div class="hangingIcon">
                        <div> - </div>
                    </div>
                    <div class="mr-12 text-white"> 3.69 GBP </div>
                    <div class="text-white bg-landing-page-dark px-4 py-2">
                        Low cost transfer
                        <span class="text-primary-light"> &#9660; </span>
                    </div>
                    <div class="text-white opacity-60 ml-4"> fee </div>
                </div>
                <div class="flex my-3 pl-12">
                    <div class="hangingIcon">
                        <div> + </div>
                    </div>
                    <div class="mr-12 text-white opacity-60"> 996.31 GBP </div>
                    <div class="text-white opacity-60"> Amount we'll convert </div>
                </div>
                <div class="flex my-3 pl-12">
                    <div class="hangingIcon">
                        <div> x </div>
                    </div>
                    <div class="mr-12 text-primary-light"> 1.19753 </div>
                    <div class="text-white opacity-60 underline cursor-pointer hover:text-primary-light"> Guaranteed rate (2 hrs) </div>
                </div>
                <div class="flex">
                    <div class="bg-white py-2 w-full">
                        <div class="text-lg px-4 text-text-gray opacity-60"> Recipient gets </div>
                        <input type="tel" value="1,193.11" class="px-4 py-2 outline outline-none text-2xl w-full" />
                    </div>
                    <div class="bg-landing-page-dark cursor-pointer flex items-center justify-center w-6/12 hover:border hover:border-white hover:border-2">
                        <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                        <div class="px-4 text-3xl font-bold text-white"> EUR </div>
                        <div class="text-primary-light">  &#9660; </div>
                    </div>
                </div>
                <div class="mt-8 hidden md:grid grid-cols-2 divide-x divide-primary-dark text-center text-white">
                    <div class="pr-4">
                        <div class="text-white opacity-60 text-md"> You could save vs banks </div>
                        <div class="text-lg"> 24.61 GBP </div>
                    </div>
                    <div class="pl-4">
                        <div class="text-white opacity-60 text-md"> Should arrive </div>
                        <div class="text-lg"> in 5 hours </div>
                    </div>
                </div>
                <div class="grid gap-4 md:gap-12 md:grid-cols-2 mt-8">
                    <div class="py-4 px-8 text-center cursor-pointer bg-primary-light transition ease-in-out hover:opacity-90 text-white">
                        Compare price
                    </div>
                    <div class="py-4 px-8 text-center cursor-pointer bg-green transition ease-in-out hover:opacity-90 text-white">
                        Get started
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
    name: 'LandingPage',
    data () {
        return {
            multiCurrencyAccountArr: ['Product features', 'Pricing', 'Use cases', 'Getting started', 'Protecting your money', 'Coverage'],
            moneyTransferArr: ['Send large amounts', 'Send money for students', 'About wise']
        }
    }
}
</script>