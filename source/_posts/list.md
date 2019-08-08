---
title: 软件列表
---

<script src="https://cdn.jsdelivr.net/npm/vue"></script>

### 游戏

<div class="gallery">
    <div class="img-item">
        <img src="https://i.loli.net/2019/08/08/X9QHSEqsZhmIBWj.png"/>
        <p class="title">使命召唤</p>
        <p class="desc">使命召唤</p>
    </div>

</div>

{% raw %}

<div id="list">
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
 var app = new Vue({
  el: '#list',
  data: {
    list: [
        {
        "_id": "5a76a190d542987ca6da0b97",
        "category": "视频",
        "name": "Movist",
        "description": "Mac上最好的视频播放器",
        "boughtAt": "2015-09-21T16:00:00.000Z",
        "logo": "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/6/c9/86d457e47888fda79a9082044edae.png",
        "remark": "",
        "price": 30,
        "type": "macOS"
    },
    {
        "_id": "5a76a1fe5159be7f56abffc6",
        "category": "视频",
        "name": "超级转霸DVD刻录版",
        "description": "Mac上最好的视频格式转换软件",
        "boughtAt": "2015-02-22T16:00:00.000Z",
        "logo": "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/ea/0a655fa1a387006f63d24b5144268.png",
        "remark": "",
        "price": 98,
        "type": "macOS"
    },
    {
        "_id": "5a76bcbffe66f7367b9c59a6",
        "category": "音乐",
        "name": "Logic Pro X",
        "description": "无购买时间，到已购项目左上角切换列表下载",
        "boughtAt": "1999-12-31T16:00:00.000Z",
        "logo": "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/3d/7bf4240effd3ecd083db3c031e557.png",
        "link": "",
        "remark": "左上角切换列表下载",
        "price": 1298,
        "type": "macOS"
    },
    {
        "_id": "5a76cba2590dbc6ac18a1af7",
        "category": "摄影",
        "name": "Luminar 2018",
        "description": "呼声很高的图片处理软件",
        "boughtAt": "2018-01-02T16:00:00.000Z",
        "link": "https://itunes.apple.com/cn/app/luminar-2018/id1296267339?mt=12",
        "logo": "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/c/68/e3667726fb8d1a56367fb3818a1a3.png",
        "remark": "",
        "price": 388,
        "type": "macOS"
    },
    {
        "_id": "5a7723de0e5ec27179be1fd9",
        "category": "视频",
        "name": "DataGraph",
        "description": "数学绘图软件DataGraph",
        "boughtAt": "2017-08-24T16:00:00.000Z",
        "link": "https://mp.weixin.qq.com/s?__biz=MjM5MjY0OTUzMw==&mid=2449440898&idx=1&sn=54c9bcc5d9166410befa4ff9bc7b6085&chksm=b2a838d085dfb1c6ac85baf1d538a6ad17352ca6ad6cd97895b0c72e601acaf40ec67f8887d7#rd",
        "logo": "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/7/d0/abd0e87d072c2db9aa799926e352b.png",
        "remark": "",
        "price": 588,
        "type": "macOS"
    }
    ]
  },
  computed: {
      computedList: function() {
          let data={};
          this.list.forEach(item => {
              if( data[item.category]) {
                  data[item.category].push(item);
              }else {
                  data[item.category] = [item]
              }
          });
          
          let datas = Object.keys(data).map(key => {
              return {
                  name: key,
                  children: data[key]
              }
          })
          return datas;
      }
  },
 mounted() {
     let nav = this.computedList.map((item, index)=> {
         return `<li class="nav-item nav-level-3"><a class="nav-link" href="#${item.name}"><span class="nav-number">${index + 1}.</span> <span class="nav-text">${item.name}</span></a></li>`
     }).join('\n');
  

     setTimeout(()=> {
  document.querySelectorAll('.post-toc-content > .nav')[0].innerHTML = nav;
     }, 1500)


 }
});
</script>

{% endraw %}
