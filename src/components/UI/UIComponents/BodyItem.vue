<template>
  <section class="v-body-item">
    <h2>{{ jobTitle }}</h2>
    <div class="jobDate">
      <i class="far fa-calendar-alt"></i>
      <p>{{ jobDate }}</p>
      <div class="badge" v-if="isCurrent">Current</div>
    </div>
    <p class="job-discription">
      <slot></slot>
    </p>
  </section>
</template>
<script>
export default {
  props: ["job-title", "job-date", "isCurrent"],
};
</script>

<style lang="scss" scoped>
.v-body-item {
  width: 100%;
  color: var(--textColor);
  padding: 10px 0px 15px 15px;
  border-bottom: 1px solid #eee;
  margin-top: 10px;
  h2 {
    display: block;
    font: 500 18px Roboto;
  }
  p {
    font: 400 15px Roboto;
    margin: 10px 0;
  }
  i {
    font-size: 18px;
    margin-right: 10px;
  }
  .jobDate {
    display: flex;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    color: #009688;
    .badge {
      color: #fafafa;
      background-color: #009688;
      margin: 0 10px;
      padding: 2px 7px;
      border-radius: 5px;
      font-size: 15px;
    }
  }
  .job-discription {
    line-height: 1.5rem;
    color: var(--textColor);
  }
}
</style>
