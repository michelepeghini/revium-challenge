<template>
  <div class="intro-text">
    <div class="intro-text__title" v-html="title"></div>
    <div class="intro-text__content" v-html="content"></div>
  </div>
</template>

<script>
export default {
  name: "IntroText",
  data: () => ({
    title: "<h2>My title</h2>",
    content: `<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus laoreet lobortis auctor. Etiam iaculis felis at velit tincidunt porta. Nunc rutrum ullamcorper porta. Praesent eleifend lorem id metus euismod condimentum. Nullam venenatis lorem vel laoreet gravida. Nam vel augue sed augue mollis tincidunt. Fusce eget ex a ante fringilla placerat ac pellentesque enim. Aliquam efficitur, nibh dictum malesuada convallis, turpis magna sollicitudin orci, tincidunt dictum sem nunc vel ex.Aenean ac massa non erat ultricies vehicula. Ut non quam suscipit, hendrerit tortor sit amet, aliquam enim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas dictum, nunc quis iaculis porttitor, mauris massa rhoncus mi, id sollicitudin dui est nec urna. Suspendisse libero sapien, ultrices vitae sem quis, pharetra molestie lectus. Nam viverra ullamcorper neque, semper dignissim ipsum consectetur laoreet. Proin eleifend ante ac lectus tincidunt egestas. Aliquam sed odio hendrerit, ultricies ipsum id, vulputate diam. Sed hendrerit purus ut dolor maximus fermentum. Sed orci magna, pretium vehicula enim posuere, ultricies molestie enim. Phasellus sed semper mi. Praesent vel consectetur sem.</p>
      <p>Integer erat risus, posuere sit amet risus vitae, placerat dictum velit. Nullam vitae nibh in augue consequat tempor. Etiam id libero gravida, mollis urna tempor, iaculis nisi. Nam commodo vel mauris quis congue. Nullam eu semper ligula, ut eleifend neque. Nulla ornare tristique erat, in rutrum risus interdum eget. Nulla bibendum sed velit ut vestibulum.</p>
      <p>Vivamus porttitor urna vitae commodo pretium. Nam enim lacus, venenatis at ante eget, sodales varius justo. Aenean at iaculis libero. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Vivamus tristique quis leo vitae euismod. Sed sit amet odio quis magna aliquet feugiat. Interdum et malesuada fames ac ante ipsum primis in faucibus. Cras varius est tortor, vel consectetur massa varius ac. Sed hendrerit tincidunt dui at commodo. Etiam eget odio nulla. Cras at rhoncus erat. Nullam ante massa, volutpat eget erat nec, sollicitudin maximus eros.</p>
      <p>Nulla sollicitudin arcu a blandit ultrices. Etiam a mi metus. Aliquam elementum sit amet eros vel scelerisque. Nunc non sapien vel arcu tincidunt aliquam sit amet ac eros. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus et arcu et erat aliquet venenatis vitae eget purus. Ut ac ex odio. Suspendisse consectetur, felis suscipit molestie lacinia, libero neque aliquet tortor, a pulvinar justo nunc ac tortor. Ut eu est id orci fermentum volutpat. Proin in rhoncus urna. Aliquam at lectus a ipsum sodales ornare tristique tincidunt velit.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus laoreet lobortis auctor. Etiam iaculis felis at velit tincidunt porta. Nunc rutrum ullamcorper porta. Praesent eleifend lorem id metus euismod condimentum. Nullam venenatis lorem vel laoreet gravida. Nam vel augue sed augue mollis tincidunt. Fusce eget ex a ante fringilla placerat ac pellentesque enim. Aliquam efficitur, nibh dictum malesuada convallis, turpis magna sollicitudin orci, tincidunt dictum sem nunc vel ex.Aenean ac massa non erat ultricies vehicula. Ut non quam suscipit, hendrerit tortor sit amet, aliquam enim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas dictum, nunc quis iaculis porttitor, mauris massa rhoncus mi, id sollicitudin dui est nec urna. Suspendisse libero sapien, ultrices vitae sem quis, pharetra molestie lectus. Nam viverra ullamcorper neque, semper dignissim ipsum consectetur laoreet. Proin eleifend ante ac lectus tincidunt egestas. Aliquam sed odio hendrerit, ultricies ipsum id, vulputate diam. Sed hendrerit purus ut dolor maximus fermentum. Sed orci magna, pretium vehicula enim posuere, ultricies molestie enim. Phasellus sed semper mi. Praesent vel consectetur sem.</p>
      <p>Integer erat risus, posuere sit amet risus vitae, placerat dictum velit. Nullam vitae nibh in augue consequat tempor. Etiam id libero gravida, mollis urna tempor, iaculis nisi. Nam commodo vel mauris quis congue. Nullam eu semper ligula, ut eleifend neque. Nulla ornare tristique erat, in rutrum risus interdum eget. Nulla bibendum sed velit ut vestibulum.</p>
      <p>Vivamus porttitor urna vitae commodo pretium. Nam enim lacus, venenatis at ante eget, sodales varius justo. Aenean at iaculis libero. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Vivamus tristique quis leo vitae euismod. Sed sit amet odio quis magna aliquet feugiat. Interdum et malesuada fames ac ante ipsum primis in faucibus. Cras varius est tortor, vel consectetur massa varius ac. Sed hendrerit tincidunt dui at commodo. Etiam eget odio nulla. Cras at rhoncus erat. Nullam ante massa, volutpat eget erat nec, sollicitudin maximus eros.</p>
      <p>Nulla sollicitudin arcu a blandit ultrices. Etiam a mi metus. Aliquam elementum sit amet eros vel scelerisque. Nunc non sapien vel arcu tincidunt aliquam sit amet ac eros. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus et arcu et erat aliquet venenatis vitae eget purus. Ut ac ex odio. Suspendisse consectetur, felis suscipit molestie lacinia, libero neque aliquet tortor, a pulvinar justo nunc ac tortor. Ut eu est id orci fermentum volutpat. Proin in rhoncus urna. Aliquam at lectus a ipsum sodales ornare tristique tincidunt velit.</p>`
  })
};
</script>


<style scoped lang="stylus">
.intro-text {
  max-width: 60%;
  margin: 20px auto;

  @media screen and (max-width: 768px) {
    max-width: 90%;
  }

  &__title {
    margin: 0 auto 30px auto;
  }

  &__content {
    text-align: justify;
  }
}
</style>
