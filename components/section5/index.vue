<template>
  <div>
    <div id="maindiv">
      <div id="div1">&nbsp;{{textData}}</div>
      <div id="div2">&nbsp;{{textData}}</div>
    </div>

    <!-- <div>horizontal carousel</div> -->
    <section class="card">
      <div class="card--content" v-for="i in 10" :key="i">
        <v-img
          lazy-src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80"
          src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80"
          height="400"
        >
          <v-row align="end" justify="center" class="fill-height">
            <v-col class="text-center white--text">
              <div>{{"תל אביב - יפו"}}</div>
              <div class="mx-auto" :style="{width:'20px',height:'1px',border:'1px solid white'}"></div>
              <div>{{"42 מרכזי קניות ומשרדים"}}</div>
            </v-col>
          </v-row>
        </v-img>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  computed: {
    textData() {
      return "hello ** lorem ipsum dolore emet ** lorem ipsum dolore emet** lorem ipsum dolore emet ** lorem ipsum dolore emet ** lorem ipsum dolore emet ** lorem ipsum dolore emet ";
    }
  }
};
</script>

<style scoped lang="scss">
#maindiv {
  width: 100%;
  border: 2px solid black;
  overflow: hidden;
  white-space: nowrap;
  background-color: black;
  color: white;
  font-size: 20px;
}

#div1 {
  display: inline-block;
  animation: marquee 20s linear infinite;
}

#div2 {
  display: inline-block;
  animation: marquee2 20s linear infinite;
  animation-delay: 10s;
}

@keyframes marquee {
  from {
    transform: translateX(100%);
  }
  to {
    transform: translateX(-100%);
  }
}

@keyframes marquee2 {
  from {
    transform: translateX(0%);
  }
  to {
    transform: translateX(-200%);
  }
}

.card {
  display: flex;
  min-width: 100%;
  min-height: 200px;
  overflow-x: auto;
}

.card::-webkit-scrollbar {
  display: none;
}
.card--content {
  min-width: 300px;
  margin: 10px;
}

.card--content img {
  width: 100%;
  height: 100%;
}
</style>