---
layout: two-cols
---

<Understand3DScenesHeadline />

::left::

<div class="w-full h-23"></div>

````md magic-move {lines: true}
```vue {12-15}
<script setup lang="ts">
import { TresCanvas } from '@tresjs/core'
import { OrbitControls } from '@tresjs/cientos'
</script>

<template>
  <TresCanvas clear-color="E1F4FF">
    <TresGridHelper />
    <TresAxesHelper />
    <TresPerspectiveCamera :position="[-5, 5, -2]" />
    <OrbitControls />
    <TresAmbientLight :intensity="0.5" color="#fff" />
    <TresDirectionalLight :intensity="1.2"
      :position="[-0.5, 3, 5]"
    />
  </TresCanvas>
</template>
```
````

::right::
