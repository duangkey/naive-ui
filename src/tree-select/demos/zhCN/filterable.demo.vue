<markdown>
# 可过滤
</markdown>

<template>
  <n-space vertical>
    <n-tree-select
      filterable
      :options="options"
      default-value="Drive My Car"
      clearable
    />
    <n-tree-select
      multiple
      checkable
      filterable
      :clear-filter-after-select="false"
      :options="options"
      :default-value="['Norwegian Wood']"
      clearable
    />
  </n-space>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup () {
    return {
      options: [
        {
          label: 'Rubber Soul',
          key: 'Rubber Soul',
          children: []
        },
        {
          label: 'Let It Be',
          key: 'Let It Be Album',
          children: [
            {
              label: 'Two Of Us',
              key: 'Two Of Us'
            },
            {
              label: 'Dig A Pony',
              key: 'Dig A Pony'
            },
            {
              label: 'Across The Universe',
              key: 'Across The Universe'
            },
            {
              label: 'I Me Mine',
              key: 'I Me Mine'
            },
            {
              label: 'Dig It',
              key: 'Dig It'
            },
            {
              label: 'Let It Be',
              key: 'Let It Be'
            },
            {
              label: 'Maggie Mae',
              key: 'Maggie Mae'
            },
            {
              label: "I've Got A Feeling",
              key: "I've Got A Feeling"
            },
            {
              label: 'One After 909',
              key: 'One After 909'
            },
            {
              label: 'The Long And Winding Road',
              key: 'The Long And Winding Road'
            },
            {
              label: 'For You Blue',
              key: 'For You Blue'
            },
            {
              label: 'Get Back',
              key: 'Get Back'
            }
          ]
        }
      ]
    }
  }
})
</script>
