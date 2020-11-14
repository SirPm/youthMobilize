<template>
  <Header />
  <BelowHeader />
  <EndSarsVideo />
  <TrendingTopics />
  <Communities />
  <MeetTheLaw />
  <HealthTips />
  <Footer />
</template>

<script>
import Header from '../components/Header';
import BelowHeader from '../components/BelowHeader';
import EndSarsVideo from '../components/EndSarsVideo';
import TrendingTopics from '../components/TrendingTopics';
import Communities from '../components/Communities';
import MeetTheLaw from '../components/MeetTheLaw';
import HealthTips from '../components/HealthTips';
import Footer from '../components/Footer';

export default {
    name: 'Homepage',
    components: {
    Header,
    BelowHeader,
    EndSarsVideo,
    TrendingTopics,
    Communities,
    MeetTheLaw,
    HealthTips,
    Footer
  }
}
</script>

<style scoped>

</style>