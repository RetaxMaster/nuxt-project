<template>
    <div>
        <h1>Hola :3</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Consectetur, totam obcaecati reiciendis aliquid tempora cumque dolorem mollitia dolores odit veritatis, fugit voluptatum eligendi iure corrupti. Blanditiis repellat aliquam eveniet nam.</p>
    </div>
</template>

<script>
export default {
  
  head() {
    return {

      title: "About - Posts",

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