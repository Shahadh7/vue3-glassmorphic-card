#  Glassmorphic Card

Customizable glassmorphic card component for your Vue3 projects. It allows you to easily create beautiful and flexible cards with a frosted glass effect and edit their styles to match your design needs.

## Features:

- Customize everything: Change background color, border radius, box shadow, blur strength, and border color to match your design.

- Easy to use: Just drop the glass-card component into your code and set the desired props.

- Slot-based content: Put any content you want inside the card, including text, images, or other components.


## Installation:

```bash
npm install vue3-glassmorphic-card
```

## Basic Usage: 

Import the glass card component into your Vue project and use it with props to customize its appearance:

```
<template>
  <div>
    <glass-card
      backgroundColor="rgba(0, 255, 0, 0.2)"
      borderRadius="20px"
      boxShadow="0 8px 40px rgba(0, 0, 0, 0.2)"
      backdropBlur="2px"
    >
      This is a customizable glassmorphic card!
    </glass-card>
  </div>
</template>

<script setup>
import GlassCard from 'vue3-glassmorphic-card';

</script>
```

## LICENSE

[MIT](https://choosealicense.com/licenses/mit/) © Shahadh

