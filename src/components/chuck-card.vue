Vue.component('chuck-card', {
    props: ['iconUrl', 'value'],
    template: `
      <div class="col-md-4 col-sm-6 mb-4">
        <div class="card h-100">
          <img :src="iconUrl" class="card-img-top" alt="...">
          <div class="card-body">
            <p class="card-text">{{ value }}</p>
          </div>
        </div>
      </div>
    `
  });
  
  new Vue({
    el: '#app',
    data: {
      chuck: [
        { iconUrl: 'https://upload.wikimedia.org/wikipedia/commons/3/30/Chuck_Norris_May_2015.jpg', value: "Chuck Norris can skydive into outer space." },
        { iconUrl: 'https://assets.chucknorris.host/img/avatar/chuck-norris.png', value: "The chief export of Chuck Norris is pain." },
        { iconUrl: 'https://assets.chucknorris.host/img/avatar/chuck-norris.png', value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { iconUrl: 'https://assets.chucknorris.host/img/avatar/chuck-norris.png', value: "Time waits for no man. Unless that man is Chuck Norris." },
        { iconUrl: 'https://assets.chucknorris.host/img/avatar/chuck-norris.png', value: "If you spell Chuck Norris in Scrabble, you win. Forever." }
      ]
    }
  });
  