<template lang="pug">
  v-layout(column justify-center align-center)
    v-flex(xs12 sm8 md6)
      div
        h1.title
          | This is product title
        p.description
          | This is product description
        .links
          a(href='#' target='_blank')
            | Add to shoping cart
          br
          a(href='#' target='_blank')
            | Buy it Now
</template>
