<template>
    <div 
        class="glass-card" 
        :style="{ ...styles }"
    >
        <slot></slot>
    </div>
</template>

<script setup>
import { computed } from "vue"


const props = defineProps({
    backgroundColor: {
      type: String,
      default: 'rgba(255, 255, 255, 0.2)',
    },
    borderRadius: {
      type: String,
      default: '10px',
    },
    boxShadow: {
      type: String,
      default: '0 4px 30px rgba(0, 0, 0, 0.1)',
    },
    backdropBlur: {
      type: String,
      default: '5px',
    },
    borderColor: {
      type: String,
      default: 'rgba(255, 255, 255, 0.18)',
    },
    width: {
        type: String,
        default: '20rem'
    },
    padding: {
        type: String,
        default: '16px'
    }    
})

const styles = computed(()=> {
    return {
        backgroundColor: props.backgroundColor,
        borderRadius: props.borderRadius,
        boxShadow: props.boxShadow,
        backdropFilter: `blur(${props.backdropBlur})`,
        '-webkit-backdrop-filter': `blur(${props.backdropBlur})`,
        border: `1px solid ${props.borderColor}`,
        padding: `${props.padding}`,
        width: `${props.width}`
    };
})

</script>

<style scoped>
.glass-card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
</style>