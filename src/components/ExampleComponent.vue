<template>
  <div class="row" style="display: flex; min-width: 700px; width: 90%">
    <q-calendar-day ref="calender" v-model="selectedDate" view="week" animated bordered>
    </q-calendar-day>
  </div>
</template>

<script setup lang="ts">
import { QCalendarDay } from '@quasar/quasar-ui-qcalendar/dist/QCalendarDay.esm.js';
import { ref } from 'vue';
const { today } = QCalendarDay;
const selectedDate = ref(today);
const calender = ref(null);
</script>
