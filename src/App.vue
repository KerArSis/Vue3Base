<script>
  export default{
    data(){
      return{
        date: '1'
      }
    },
    methods: {
      show: function(){
        let date = this.dayOfWeek(this.date);
        const dayOfWeekDigit = new Date().getDay();
        let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
        alert(date);
      },
      dayOfWeek: function(date){
        let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
        return days[date];
      },
    }
  }
</script>

<template>
  <button class="button" @click="show">Day</button>
  {{ dayOfWeekDigit }}
</template>

<style>

</style>
