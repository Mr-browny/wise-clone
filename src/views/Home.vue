<template>
  <div class="home">
    <MessageAlert/>
    <Landingpage/>
    <AvailableSection/>
    <UseCaseSection/>
    <GetStarted/>
    <CustomerCare/>
    <Security/>
    <Coverage/>
    <Faqs/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import MessageAlert from '@/components/MessageAlert.vue'
import Landingpage from '@/components/Landingpage.vue'
import AvailableSection from '@/components/AvailableSection.vue'
import UseCaseSection from '@/components/UseCaseSection.vue'
import GetStarted from '@/components/GetStarted.vue'
import CustomerCare from '@/components/CustomerCare.vue'
import Security from '@/components/Security.vue'
import Coverage from '@/components/Coverage.vue'
import Faqs from '@/components/Faqs.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    MessageAlert,
    Landingpage,
    AvailableSection,
    UseCaseSection,
    GetStarted,
    CustomerCare,
    Security,
    Coverage,
    Faqs,
    Footer,
  }
}
</script>
