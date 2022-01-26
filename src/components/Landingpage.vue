<template>
    <div class="bg-primary px-10 md:px-64">
        <div class="flex justify-between py-10">
            <div class="flex justify-evenly items-baseline">
                <img src="https://wise.com/public-resources/assets/logos/wise/brand_logo_inverse.svg" alt="Wise" class="pr-4">
                <div class="xs:hidden sm:block grid grid-cols-3 divide-x text-white font-bold">
                    <div class="text-2xl pr-4 text-primary-light cursor-pointer"> Personal </div>
                    <div class="text-2xl pl-4 cursor-pointer"> Business </div>
                </div>
            </div>
            <div class="w-6/12 pt-2 flex justify-evenly items-baseline font-bold text-xl text-white">
                <div class="cursor-pointer"> Money transfer  &#9660;</div>
                <div class="cursor-pointer"> Multi-currency account  &#9660; </div>
                <div class="cursor-pointer"> Help </div>
                <div class="cursor-pointer"> &#127760; EN  &#9660;</div>
                <div class="cursor-pointer"> Log in</div>
                <div class="cursor-pointer"> Register </div>
            </div>
        </div>
        <div class="pt-10 pb-20 grid grid-cols-1 sm:grid-cols-2">
            <div class="flex flex-col justify-between">
                <div class="text-4xl text-white"> The cheap, fast wasy to send money <br> abroad. </div>
                <div class="grid gap-0 grid-cols-2">
                    <div>
                        Video icon
                    </div>
                    <div class="text-primary-light"> See how it works </div>
                </div>
                <div class="grid grid-cols-2">
                    <div>
                        <h3 class="text-white"> Over 12 million customers </h3>
                        <div class="expandable-link  flex items-baseline  text-primary-light font-bold cursor-pointer">
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
                        <div class="expandable-link  flex items-baseline  text-primary-light font-bold cursor-pointer">
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
            <div class="pl-56">
                <div class="flex">
                    <div class="bg-white py-2 w-full">
                        <div class="text-lg px-4 text-blue-500"> You send </div>
                        <input type="tel" value="1,000" class="px-4 py-2 outline outline-none text-2xl w-full" />
                    </div>
                    <div class="bg-blue-400 cursor-pointer flex items-center justify-center w-6/12 hover:border hover:border-white hover:border-2">
                        <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                        <div class="px-4 text-3xl font-bold text-white"> GBP </div>
                        <div class="text-primary-dark">  &#9660; </div>
                    </div>
                </div>
                <div class="flex my-4 pl-12">
                    <div class="mr-12 text-white"> 3.69 GBP </div>
                    <div class="text-white"> Low cost transfer  &#9660; </div>
                    <div> fee </div>
                </div>
                <div class="flex my-4 pl-12">
                    <div class="mr-12 text-text-gray"> 996.31 GBP </div>
                    <div class="text-text-gray"> Amount we'll convert </div>
                </div>
                <div class="flex my-4 pl-12">
                    <div class="mr-12"> 1.19753 </div>
                    <div class="text-text-gray underline cursor-pointer hover:text-primary-light"> Guaranteed rate (2 hrs) </div>
                </div>
                <div class="flex">
                    <div class="bg-white py-2 w-full">
                        <div class="text-lg px-4 text-blue-500"> Recipient gets </div>
                        <input type="tel" value="1,193.11" class="px-4 py-2 outline outline-none text-2xl w-full" />
                    </div>
                    <div class="bg-blue-400 cursor-pointer flex items-center justify-center w-6/12 hover:border hover:border-white hover:border-2">
                        <img src="@/assets/icons/icon1.png" alt="icon" width="20" height="20" />
                        <div class="px-4 text-3xl font-bold text-white"> EUR </div>
                        <div class="text-primary-dark">  &#9660; </div>
                    </div>
                </div>
                <div class="mt-8 grid grid-cols-2 divide-x text-center text-white">
                    <div class="text-lg pr-4">
                        <div> You could save vs banks </div>
                        <div> 24.61 GBP </div>
                    </div>
                    <div class="text-lg pl-4">
                        <div> Should arrive </div>
                        <div> in 5 hours </div>
                    </div>
                </div>
                <div class="grid gap-12 grid-cols-2 mt-8">
                    <div class="py-4 px-8 text-center cursor-pointer bg-primary-light hover:bg-primary-dark text-white">
                        Compare price
                    </div>
                    <div class="py-4 px-8 text-center cursor-pointer bg-green hover:bg-green-dark text-white">
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
    name: 'LandingPage'
}
</script>