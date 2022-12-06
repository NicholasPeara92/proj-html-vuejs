<script>
export default {};
</script>
<template>
  <div id="spacer"></div>
</template>

<style lang="scss" scoped>
#spacer {
  position: relative;
}
#spacer::after {
  content: "";
  position: absolute;
  left: 15px;
  height: 6px;
  width: 40px;
  background: linear-gradient(
    270deg,
    #0edaa0ff,
    #30dc90ff,
    #51dd81ff,
    #73df71ff,
    #94e061ff
  );
}
#spacer::before {
  content: "";
  position: absolute;
  height: 6px;
  width: 10px;
  background: linear-gradient(
    270deg,
    #0edaa0ff,
    #30dc90ff,
    #51dd81ff,
    #73df71ff,
    #94e061ff
  );
}
</style>
