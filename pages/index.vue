<template>
  <div class="container">
    <div class="row">
      <!--Left Menu block-->
      <LeftMenu />
      <!--middle block-->
      <div class="col-lg-6 col-md-11 col-10">
        <main>
          <div class="first-part">
            <div>
              <a class="home">Beranda ({{ $store.state.counter }})</a>
            </div>
            <div>
              <i class="far fa-star"></i>
            </div>
          </div>
          <div class="whats-happening">
            <form @submit="onSubmit">
              <div class="post-blocks">
                <div class="post-profile">
                  <img src="/img_avatar.png" class="avatar" alt="Avatar" />
                </div>
                <textarea
                  class="post-form"
                  placeholder="Apa yang sedang terjadi?"
                  v-model="tweet"
                  name="tweet"
                  v-on:keyup="triggerKey"
                ></textarea>
              </div>
              <div class="post-icons">
                <div class="first-post-icons">
                  <i>
                    <font-awesome-icon :icon="['fas', 'fa-image']" />
                  </i>
                  <i>
                    <font-awesome-icon :icon="['fas', 'fa-gift']" />
                  </i>
                  <i>
                    <font-awesome-icon :icon="['fas', 'fa-signal']" />
                  </i>
                  <i>
                    <font-awesome-icon :icon="['fas', 'fa-smile']" />
                  </i>
                </div>
                <div class="second-post-icons">
                  <i class="far fa-circle"></i>
                  <i class="fas fa-plus-circle"></i>
                  <input @click="$store.commit('increment')"
                    type="submit"
                    value="Tweet"
                    id="submit-tweet"
                    class="btn btn-primary btn-sm tweeterBtn" disabled
                  />
                </div>
              </div>
            </form>
          </div>
        </main>
        <!--TWEEEEEETS-->
        <section id="tweets">
          <!--1 tweet-->
          <div class="tweet-1" v-for="item in items" :key="item.id">
            <div class="tweet-img">
              <img src="/img_avatar.png" alt="Avatar" />
            </div>
            <div class="tweet-txt">
              <div class="tweet-name-date">
                <strong> Taupik Pirdian</strong>
                <span class="twitter-account"> @piridin</span> -
                <span class="date"> {{ item.date }}</span>
              </div>
              <div class="message">{{ item.tweet }}</div>
              <div class="tweet-icons">
                <i class="fas fa-image"></i>
                <i class="fas fa-gift"></i>
                <i class="fas fa-signal"></i>
                <i class="fas fa-smile"></i>
              </div>
            </div>
          </div>
        </section>
      </div>
      <!--Right  block-->
      <RightBlock />
    </div>
  </div>
</template>

<script>
let arrjson = [];
export default {
  name: "AddInformation",
  data() {
    return {
      tweet: "",
      date: "",
      items: arrjson,
    };
  },
  methods: {
    onSubmit(e) {
      e.preventDefault();
      if (!this.tweet) {
        alert("Please Type a Tweet");
        return;
      }

      var currentDate = new Date();
      var month = currentDate.getMonth();
      var date = currentDate.getDate();
      var time = currentDate.toLocaleTimeString();
      var stringDate = monthTrans(month) + " " + date + ", " + time;

      const NewInformation = {
        id: Math.floor(Math.random() * 100000),
        tweet: this.tweet,
        date: stringDate,
      };

      arrjson.push(NewInformation);
      this.tweet = "";
      document.getElementById('submit-tweet').disabled = true;

    },
    triggerKey: function(evt) {
        document.getElementById('submit-tweet').disabled = false;
    }
  },
};

function monthTrans(month) {
  switch (month) {
    case 0:
      month = "Jan";
      break;
    case 1:
      month = "Feb";
      break;
    case 2:
      month = "Mar";
      break;
    case 3:
      month = "Apr";
      break;
    case 4:
      month = "May";
      break;
    case 5:
      month = "Jun";
      break;
    case 6:
      month = "Jul";
      break;
    case 7:
      month = "Aug";
      break;
    case 8:
      month = "Sep";
      break;
    case 9:
      month = "Oct";
      break;
    case 10:
      month = "Nov";
      break;
    case 11:
      month = "Des";
      break;
  }

  return month;
}
</script>
