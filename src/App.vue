<template>
  <div>
    <intro />
    <first-steps />
    <integration />
  </div>
</template>

<script>
import FirstSteps from './components/FirstSteps'
import Integration from './components/Integration'
import Intro from './components/Intro'

export default {
  components: {
    FirstSteps,
    Integration,
    Intro
  }
}
</script>
