<template>
    <div>
         {{ description }} <select id="cars">
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