---
title: "Learning Vue.js"
date: 2023-07-20T12:26:02+05:30
# weight: 1
tags: [""]
author: "Vibhakar \"Gala\" Solanki"
showToc: true
TocOpen: false
draft: true
hidemeta: false
comments: false
description: "Desc Text."
canonicalURL: "https://canonical.url/to/page"
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: false # only hide on current single page
editPost:
    URL: "https://github.com/p0lygun/p0lygun.github.io/tree/main/content/blog"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---
# Learning Vue
first reactive SFC
```vue
<link href='https://fonts.googleapis.com/css?family=Montserrat' rel='stylesheet'>
<style>
  body {
    background-color:black;
    color:white;
    font-family: 'Montserrat';font-size: 22px;
  }
</style>

<script setup>
import { ref } from 'vue'

// component logic
// declare some reactive state here.
  const randString = ref('Start')
  function setRandomString(){
    randString.value = (Math.random() + 1).toString(36).substring(7);
    setTimeout(setRandomString, 1000);
  }
  setRandomString();
</script>

<template>
  <h1>Make me dynamic! - {{ randString.toUpperCase() }}</h1>
</template>
```

- directives
	- starts with `v-` attribute
	- is a way to bind dynamic value
	- v-bind
		- :id
		- after `:` is the argument
		- `:id` short-hand available
	- v-on
		- listen to DOM events
		- short-hand is `@`
		- so `@click` is same as `v-bind:click`
	- v-model
		- combines `v-bind` and `v-on`
		- use `object.value` to get value
	- Control flow
		- v-if, v-else, v-else-if
		- v-for
- Emits and Props
	- `defineEmits -> emit`
		- use `v-on` or `@` to catch emit
	- props are just attributes
		- use `v-bind` or `:` 


- codes
```vue
<script setup>
import { ref } from 'vue'

const count = ref(0)
function conquer(){
  count.value++;
}
</script>

<template>
  <!-- make this button work -->
  <button @click="conquer">count is: {{ count }}</button>
</template>
```