<template>
  <article class="media">
    <figure class="media-left image is-48x48">
      <img :src="'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2363297362,1082434112&fm=253&gp=0.jpg'" alt="User Avatar" style="border-radius: 5px;">

    </figure>
    <div class="media-content">
      <div class="content">
        <p>
          <strong>{{ comment.username }}</strong>
          <small class="ml-2">{{ comment.createTime | date }}</small>
          <br />
          {{ comment.content }}
        </p>
      </div>
    </div>
  </article>
</template>

<script>

export default {
  name: 'LvCommentsItem',
  props: {
    comment: {
      type: Object,
      required: true
    }
  }
}
</script>


