<template>
  <v-card class="elevation-0 transparent">
    <v-card-text class="text-center">
      <v-avatar size="150" class="justify-center text-center ">
        <img
          v-if="avatar"
          :src="require(`@/assets/crew/${avatar}`)"
          class="text-center justify-center"
        />
        <img
          v-else
          :src="require(`@/assets/other/question_dark.png`)"
          class="text-center justify-center"
        />
      </v-avatar>
    </v-card-text>
    <v-card-title
      primary-title
      class="layout justify-center text-center body-2 font-weight-bold"
    >
      {{ name }}
    </v-card-title>
    <v-card-text class="mt-n4 text-center">{{ faculty }}</v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'CrewCard',
  props: {
    name: String,
    faculty: String,
    avatar: String,
  },
};
</script>

<style scoped></style>
