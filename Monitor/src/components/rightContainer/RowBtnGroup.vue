<template>
  <div class="row_btn-group">
    <div class="btn-group btn-group-toggle" data-toggle="buttons">
      <label class="btn btn-outline-secondary active" id="raw_option">
        <input type="radio" name="options" class="data_option" /> Raw
      </label>
      <label class="btn btn-outline-secondary" id="user_option">
        <input type="radio" name="options" class="data_option" /> User
      </label>
    </div>
    <div class="btn-group">
      <button
        id="deviceDropDownBtn"
        type="button"
        class="btn btn-outline-secondary dropdown-toggle"
        data-toggle="dropdown"
        aria-haspopup="true"
        aria-expanded="false"
      >Devices</button>
      <div class="dropdown-menu device-dropdown-menu">
        <!-- <a
            class="dropdown-item location_menu aerobox-control-area"
            id="{{info.w_id}}"
        >{{info.public_info__name}}</a>-->
      </div>
    </div>
    <div class="btn-group btn-group-toggle row_dayselect" data-toggle="buttons">
      <label class="btn btn-outline-secondary active" id="todayOption">
        <input type="radio" name="options" /> Today
      </label>
      <label class="btn btn-outline-secondary" id="yesterdayOption">
        <input type="radio" name="options" /> Yesterday
      </label>
      <label class="btn btn-outline-secondary" id="thisWeekOption">
        <input type="radio" name="options" /> This Week
      </label>
      <label class="btn btn-outline-secondary" id="thisMonthOption">
        <input type="radio" name="options" /> This Month
      </label>
    </div>
  </div>
</template>
<style scoped>
.row_btn-group {
  width: 100%;
  background-color: #aaf;
  padding-top: 30px;
  margin-right: 0px;
  margin-left: 0px;
}
.row_btn-group .btn-group + .btn-group {
  margin-left: 60px;
}
@media screen and (max-width: 850px) {
  .row_btn-group {
    flex-wrap: wrap;
  }
  .row_btn-group .btn-group + .btn-group {
    margin-left: 0;
  }
  .row_btn-group .btn-group:nth-child(2) {
    margin-left: 30px;
  }
  .row_btn-group .btn-group:nth-child(3) {
    margin-top: 30px;
    display: flex;
    flex-wrap: wrap;
  }
}
@media screen and (max-width: 321px) {
  .row_btn-group .btn-group:nth-child(1) {
    margin-right: 30px;
  }
  .row_btn-group .btn-group:nth-child(2) {
    margin-top: 30px;
    margin-left: 0;
  }
}
</style>