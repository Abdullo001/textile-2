<template >
  <div class="wrapper">
    <form action="" class="search-form">
      <div>
        <input class="input-control" type="text" placeholder="Order Number" />
        <input class="input-control" type="text" placeholder="Model group" />
        <input class="input-control" type="date" />
        <input class="input-control" type="date" />
      </div>

      <div>
        <button type="reset" class="btn reset-btn">Reset</button>
        <button class="btn search-btn">Search</button>
      </div>
    </form>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.wrapper {
  margin-bottom: 16px;
  padding: 16px;
  border-radius: 6px 6px 0px 0px;
  background-color: #ffffff;
}

.search-form{
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.input-control {
  display: inline-block;
  margin-right: 12px;
  padding: 12px 0px 12px 10px;
  width: 170px;
  background: #ffffff;
  border: 1px solid #d2d3d6;
  border-radius: 6px;
}

.input-control:nth-child(4) {
  margin-right: 0;
}

.btn {
  padding: 9px 16px;

  width: 140px;
  border-radius: 6px;

  font-weight: 700;
  font-size: 16px;
  line-height: 18px;

  text-align: center;
  letter-spacing: 0.01em;
  text-transform: capitalize;
}

.reset-btn {
  margin-right: 16px;
  border: 2px solid $secondary;
  color: $secondary;
}

.search-btn {
  color: #ffffff;
  background-color: $secondary;
}
</style>