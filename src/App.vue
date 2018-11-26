<template>
  <div>
    <intro />
    <first-steps />
    <integration />
    <final />
  </div>
</template>

<script>
import Final from './components/Final'
import FirstSteps from './components/FirstSteps'
import Integration from './components/Integration'
import Intro from './components/Intro'

export default {
  components: {
    Final,
    FirstSteps,
    Integration,
    Intro
  }
}
</script>
