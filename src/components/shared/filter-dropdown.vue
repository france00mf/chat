<template>
    <div class="filter-dropdown">
         <p>{{ description }}</p> <select id="cars">
  <option value="volvo">Lastest Firs
  </option>
  <option value="saab">Saab</option>
  <option value="mercedes">Mercedes</option>
  <option value="audi">Audi</option>
</select>
    </div>
</template>

<script>
export default {
    name: 'button-add',
    props: ['description']
}
</script>

<style scoped>
.filter-dropdown{
    width: 150px;
    justify-content: space-between;
    display: flex;
}
.filter-dropdown p{
    margin: 0;
}
</style>