<script setup lang="ts">
import { Avatar, AvatarFallback, AvatarImage } from '@/components';
import { getInitials } from '@/utils';

interface PropsInterface {
  name: string
  avatar: string
  displayName?: boolean,
  ago?: string,
  size?: 'sm' | 'base' | 'lg',
  classes?: string,

}

// Define props with or without defaults
const props = withDefaults(defineProps<PropsInterface>(), {
  name: '',
  avatar: '',
  displayName: true,
  ago: '',
  size: 'sm',
  classes: '',
})
const sizeClasses = {
  sm: 'h-8 w-8 text-xs ',
  base: 'h-10 w-10 text-sm',
  lg: 'h-12 w-12 text-lg',
}
</script>
<template>
  <div :class="[
    'flex w-full mb-4 gap-2 items-center text-foreground  ',
    sizeClasses[props.size], classes
  ]">
    <Avatar :size="size" class="border">
      <AvatarImage :src="props.avatar" :alt="props.name" />
      <AvatarFallback>{{ getInitials(props.name) }}</AvatarFallback>
    </Avatar>
    <span class="flex  flex-col">
      <p v-if="displayName">
        {{ props.name }}
      </p>
      <p v-if="Boolean(ago)">
        <span class="hidden md:inline-block">•</span>
        <span>{{ ago }}</span>
      </p>
    </span>
  </div>
</template>


<style lang="scss" scoped></style>