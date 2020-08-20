<template lang="pug">
  aside.navigation
    .navigation__select-wrap
      select.navigation__select
        option Эксперт
        option Не эксперт
      img(src='').navigation__select-img

    nav.navigation__nav
      ul.navigation__list
        li.navigation__item(v-for="items of nav")
          a(:href="items.route").navigation__link
            img(:src="items.image")
            span {{items.text}}
</template>

<script>
export default {
  name: "Aside-nav",
  data() {
    return {
      nav: [
        {text:'Аналитика',image: '/',route:'/'},
        {text:'Продукт',image: '/',route:'/'},
        {text:'Пользователи',image: '/',route:'/'},
        {text:'Конструктор сайта',image: '/',route:'/'},
        {text:'Трансляции',image: '/',route:'/'},
        {text:'Рассылка',image: '/',route:'/'},
        {text:'Маркетинг',image: '/',route:'/'},
        {text:'Платежи',image: '/',route:'/'},
        {text:'Настройки',image: '/',route:'/'}
      ],
    }
  },
}
</script>

<style scoped>

</style>
