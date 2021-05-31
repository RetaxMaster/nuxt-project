<template>
  <h1>¡Una app con Nuxt!</h1>
</template>

<script>
export default {
  
  head() {
    return {

      title: "Home - Posts",

      meta: [
        {
          hid: "description",
          name: "description",
          content: "Ejemplo de sitio de posts con Nuxt"
        },
      ],

      htmlAttrs: {
        lang: "es"
      }

    }
  }

}
</script>