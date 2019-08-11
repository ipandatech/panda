---
title: 软件列表
---
<script src="https://cdn.jsdelivr.net/npm/vue"></script>


</div>
{% raw %}

<div id="list">
  <div class="search-wrapper">
    <input class="search" placeholder="此处搜索你想要的mac app" v-model="filter"/>
  </div>
    <div v-for="item in computedList">
    <template>
        <h3 :id="item.name"><a :href="'#' + item.name" class="headerlink" :title="item.name"></a>{{item.name}}</h3>
        <div class="gallery">
    <div class="img-item" v-for="child in item.children">
        <img :src="child.logo"/>
        <p class="title">{{child.name}}</p>
        <p class="desc">{{child.description}}</p>
    </div>

</div>
    </template>
    </div>
    
</div>

<script>
function getDataSetVue(data) {
    // data = JSON.parse(data);
var app = new Vue({
    el: "#list",
    data: {
      list: data,
      filter: ''
    },
    computed: {
      computedList: function() {
        let data = {};
        let list = this.list.filter(item => {
            // // return [eval(`/${this.filter}/i`)].test(item.name);
            // console.log(eval(`/${this.filter}/i`))
            // console.log(`/${this.filter}/i`)
            return item.name.indexOf(this.filter) !== -1;
        });
        list.forEach(item => {
          if (data[item.category]) {
            data[item.category].push(item);
          } else {
            data[item.category] = [item];
          }
        });

        let datas = Object.keys(data).map(key => {
          return {
            name: key,
            children: data[key]
          };
        });
        return datas;
      }
    },
    mounted() {
      let nav = this.computedList
        .map((item, index) => {
          return `<li class="nav-item nav-level-3"><a class="nav-link" href="#${
            item.name
          }"><span class="nav-number">${index +
            1}.</span> <span class="nav-text">${item.name}</span></a></li>`;
        })
        .join("\n");

      console.log(123);
      setTimeout(() => {
        document.querySelectorAll(
          ".post-toc-content > .nav"
        )[0].innerHTML = nav;
      }, 1500);
    }
  });
}
  
</script>
<script src="http://localhost:3200/apps?callback=getDataSetVue"></script>
{% endraw %}
