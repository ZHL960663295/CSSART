<template>
  <div id="app">
    <shengbeilayout />
    <shuangfeiyilayout />
    <testAround />
    <attr />
    <tieding />
  </div>
</template>

<script>
import shengbeilayout from './components/layout/shengbeilayout'
import shuangfeiyilayout from './components/layout/shuangfeiyilayout'
import testAround from './components/layout/textAround'
import attr from './components/function/attr'
import tieding from './components/background/tieding'

export default {
  name: 'App',
  components: {
    shengbeilayout,
    shuangfeiyilayout,
    testAround,
    attr,
    tieding
  }
}
</script>

<style>
*{
    margin: 0;
    padding: 0;
}
</style>
