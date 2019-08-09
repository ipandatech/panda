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
    el: "#list",
    data: {
      list: [
        {
          _id: "5a76a190d542987ca6da0b97",
          category: "视频",
          name: "Movist",
          description: "Mac上最好的视频播放器",
          boughtAt: "2015-09-21T16:00:00.000Z",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/6/c9/86d457e47888fda79a9082044edae.png",
          remark: "",
          price: 30,
          type: "macOS"
        },
        {
          _id: "5a76a1fe5159be7f56abffc6",
          category: "视频",
          name: "超级转霸DVD刻录版",
          description: "Mac上最好的视频格式转换软件",
          boughtAt: "2015-02-22T16:00:00.000Z",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/ea/0a655fa1a387006f63d24b5144268.png",
          remark: "",
          price: 98,
          type: "macOS"
        },
        {
          _id: "5a76bcbffe66f7367b9c59a6",
          category: "音乐",
          name: "Logic Pro X",
          description: "无购买时间，到已购项目左上角切换列表下载",
          boughtAt: "1999-12-31T16:00:00.000Z",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/3d/7bf4240effd3ecd083db3c031e557.png",
          link: "",
          remark: "左上角切换列表下载",
          price: 1298,
          type: "macOS"
        },
        {
          _id: "5a76cba2590dbc6ac18a1af7",
          category: "摄影",
          name: "Luminar 2018",
          description: "呼声很高的图片处理软件",
          boughtAt: "2018-01-02T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/luminar-2018/id1296267339?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/c/68/e3667726fb8d1a56367fb3818a1a3.png",
          remark: "",
          price: 388,
          type: "macOS"
        },
        {
          _id: "5a7723de0e5ec27179be1fd9",
          category: "视频",
          name: "DataGraph",
          description: "数学绘图软件DataGraph",
          boughtAt: "2017-08-24T16:00:00.000Z",
          link:
            "https://mp.weixin.qq.com/s?__biz=MjM5MjY0OTUzMw==&mid=2449440898&idx=1&sn=54c9bcc5d9166410befa4ff9bc7b6085&chksm=b2a838d085dfb1c6ac85baf1d538a6ad17352ca6ad6cd97895b0c72e601acaf40ec67f8887d7#rd",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/7/d0/abd0e87d072c2db9aa799926e352b.png",
          remark: "",
          price: 588,
          type: "macOS"
        },
        {
          _id: "5a781e4ccac520302220639a",
          category: "视频",
          name: "Smart Coverter Pro 2",
          description: "视频格式转换软件",
          boughtAt: "2017-08-24T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/smart-converter-pro-2/id660234210?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/4/f4/d8cdc19d6bc33a9d6a6984977ebc6.png",
          remark: "",
          price: 98,
          type: "macOS"
        },
        {
          _id: "5a782245cac520302220639f",
          category: "视频",
          name: "Final Cut Pro X",
          description: "无购买时间，到已购项目左上角切换列表下载",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/6/c3/57594e34ac47ff056c37a18e1b066.png",
          remark: "",
          price: 1998,
          type: "macOS"
        },
        {
          _id: "5a78227bcac52030222063a1",
          category: "视频",
          name: "Motion",
          description: "无购买时间，到已购项目左上角切换列表下载",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/f/f7/19555002c401d639c15a17081bed6.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a7859c5f3b175062048860e",
          category: "视频",
          name: "Compressor",
          description: "无购买时间，到已购项目左上角切换列表下载",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/1/9e/7d73621f8027ed2bc4e8d784c344e.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a785b66f3b1750620488611",
          category: "视频",
          name: "ScreenFlow 8",
          description: "Mac上最好用的录屏软件",
          boughtAt: "2018-08-16T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/screenflow-7/id1223627207?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/1/1b/2444809728be69aaf377830dac144.png",
          remark: "",
          price: 848,
          type: "macOS"
        },
        {
          _id: "5a78683531c90f3ce5b81012",
          category: "视频",
          name: "可意视频Pro",
          description: "视频播放器，和Movist旗鼓相当",
          boughtAt: "2016-01-10T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/6/b8/6412560ca23cbd01ff0ba9b657753.png",
          remark: "",
          price: 12,
          type: "macOS"
        },
        {
          _id: "5a7868e831c90f3ce5b81015",
          category: "视频",
          name: "Mplayerx",
          description: "轻量级视频播放器",
          boughtAt: "2015-07-22T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/mplayerx/id421131143?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/5a/d417b0549ea4716f00ee2be19fdc8.png",
          remark: "",
          price: 12,
          type: "macOS"
        },
        {
          _id: "5a7869eb31c90f3ce5b81018",
          category: "视频",
          name: "SendToX",
          description: "将老版本Final文件转换到X可以打开的软件",
          boughtAt: "2016-03-30T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/sendtox/id496926258?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/b8/fb2a83bd35f8838593f7f9da7e53b.png",
          remark: "",
          price: 68,
          type: "macOS"
        },
        {
          _id: "5a786a5131c90f3ce5b81019",
          category: "视频",
          name: "Premiere SRT",
          description: "将STR字幕文件导入PR里面进行使用的软件",
          boughtAt: "2016-10-19T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/premiere-srt/id993381506?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/34/3c306eb6392111e955e965137815e.png",
          remark: "",
          price: 68,
          type: "macOS"
        },
        {
          _id: "5a786ef9a00e5c713ad34b12",
          category: "视频",
          name: "Subtitle Edit Pro",
          description: "Mac上的字幕编辑软件，十分方便",
          boughtAt: "2016-10-19T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/subtitle-edit-pro/id1065306078?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/59/a1c1982d9b6d3cd627bf7a2513fdd.png",
          remark: "",
          price: 198,
          type: "macOS"
        },
        {
          _id: "5a786f78a00e5c713ad34b13",
          category: "视频",
          name: "Final SRT",
          description: "将STR字幕文件导入Final里面进行使用的软件 ",
          boughtAt: "2016-09-19T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/final-srt/id876201194?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/9/37/cf05bc6f9c2269c7595b555645ff0.png",
          remark: "",
          price: 98,
          type: "macOS"
        },
        {
          _id: "5a786fc3a00e5c713ad34b14",
          category: "视频",
          name: "XtoCC",
          description: "将最新版本“X版本”Final文件转换到7可以打开的软件",
          boughtAt: "2016-12-12T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/xtocc/id487899517?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/4/f8/1f1251c2ecd9e11f0a264818bfec8.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a787034a00e5c713ad34b15",
          category: "视频",
          name: "CameraBag Cinema",
          description: "视频滤镜，美化工具",
          boughtAt: "2016-12-31T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/camerabag-cinema/id1101039207?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/e/58/42b9393b002ebe18885c3f9c33e2b.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a78708ba00e5c713ad34b16",
          category: "视频",
          name: "完美影音",
          description: "视频播放",
          boughtAt: "2017-07-17T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/%E5%AE%8C%E7%BE%8E%E5%BD%B1%E9%9F%B3-%E5%AE%8C%E7%BE%8E%E6%92%AD%E6%94%BE%E9%AB%98%E6%B8%85%E8%A7%86%E9%A2%91-%E4%BA%AB%E5%8F%97%E5%9C%A8%E5%AE%B6%E7%9C%8B%E7%94%B5%E5%BD%B1/id1132551837?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/d/27/6b37be32ff81507142f28490fe8f9.png",
          remark: "",
          price: 68,
          type: "macOS"
        },
        {
          _id: "5a78773ae4290a7ea5910488",
          category: "音乐",
          name: "Djay Pro ",
          description: "非常适合音乐人士使用的DJ工具",
          boughtAt: "2016-01-11T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/4/d6/b6657f65f500460c09637bbc5563d.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a7877fee4290a7ea5910489",
          category: "音乐",
          name: "myTuner Radio Pro",
          description: "全球最火FM电台收音机",
          boughtAt: "2016-01-10T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/mytuner-radio-pro-%E5%85%A8%E7%90%83%E6%9C%80%E7%81%ABfm%E7%94%B5%E5%8F%B0%E6%94%B6%E9%9F%B3%E6%9C%BA/id808285143?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/64/869cc2d4832f7b1233fb4b595877d.png",
          remark: "",
          price: 68,
          type: "macOS"
        },
        {
          _id: "5a78784de4290a7ea591048a",
          category: "音乐",
          name: "MainStag3",
          description: "配合LogicX使用，DJ现场控制神器",
          boughtAt: "2016-04-04T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/mainstage-3/id634159523?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/7/6c/ec31eef7b3f03bfe138e36766fe20.png",
          remark: "",
          price: 198,
          type: "macOS"
        },
        {
          _id: "5a7878c1e4290a7ea591048b",
          category: "音乐",
          name: "Soundboard",
          description: "音效加强器。",
          boughtAt: "2016-12-31T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/soundboard/id414067156?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/3/d9/3ed9a85ccf63c6932c6de98175e94.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a787906e4290a7ea591048c",
          category: "音乐",
          name: "Capo3",
          description: "音谱学习软件",
          boughtAt: "2016-12-31T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/capo-3/id696977615?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/7/1e/827faafc1a528f9ee00522ed02a28.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a787983e4290a7ea591048d",
          category: "音乐",
          name: "Noizio",
          description: "还你一个安静的私人空间，降噪工具",
          boughtAt: "2015-10-02T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/noizio/id928871589?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/7/cd/ecf60634da68dd848c65b29a46466.png",
          remark: "",
          price: 18,
          type: "macOS"
        },
        {
          _id: "5a7879bfe4290a7ea591048e",
          category: "音乐",
          name: "Audio Converter Pro",
          description: "音频格式转换软件",
          boughtAt: "2017-07-17T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/audio-converter-pro/id698196505?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/5/eb/8ef244386fc0ed64114af00bf2372.png",
          remark: "",
          price: 45,
          type: "macOS"
        },
        {
          _id: "5a787a21e4290a7ea591048f",
          category: "图形与设计",
          name: "我的画笔 MyBrushes",
          description: "独特的，能回放整个绘画过程的工具",
          boughtAt: "2016-02-26T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/%E6%88%91%E7%9A%84%E7%94%BB%E7%AC%94-mybrushes-%E4%B8%93%E6%B3%A8%E4%B8%AD%E5%9B%BD%E7%94%BB-%E7%B4%A0%E6%8F%8F-%E6%B0%B4%E5%BD%A9%E5%92%8C%E4%B9%A6%E6%B3%95%E8%89%BA%E6%9C%AF/id676028900?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/7/2b/682263a2f243016a8b0f1c153672b.png",
          remark: "",
          price: 128,
          type: "macOS"
        },
        {
          _id: "5a787aa4e4290a7ea5910492",
          category: "摄影",
          name: "泼辣修图",
          description: "小而强大的修图/滤镜工具",
          boughtAt: "2016-01-28T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/%E6%B3%BC%E8%BE%A3%E4%BF%AE%E5%9B%BE/id1058273036?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/2/69/805372764938ad70e7b1cba1543c1.png",
          remark: "",
          price: 128,
          type: "macOS"
        },
        {
          _id: "5a787b57e4290a7ea5910493",
          category: "摄影",
          name: "Aurora HDR",
          description: "强大的HDR工具",
          boughtAt: "2015-12-21T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/6/cb/896028901433efbef0069caea5e40.png",
          remark: "",
          price: 258,
          type: "macOS"
        },
        {
          _id: "5a787c75e4290a7ea5910494",
          category: "图形与设计",
          name: "Hexels Pro",
          description: "六边形绘图设计工具",
          boughtAt: "2015-12-16T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/3/03/275f38c2dfb01556d6acf70709686.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a787ce8e4290a7ea5910495",
          category: "图形与设计",
          name: "Flinto",
          description: "老版本Flinto",
          boughtAt: "2016-12-12T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/63/fcd5bb11be63cd0175e167ec98622.png",
          remark: "",
          price: 488,
          type: "macOS"
        },
        {
          _id: "5a787e2ae4290a7ea5910496",
          category: "图形与设计",
          name: "Sketch 5",
          description: "会员专享，联系客服获取下作方法，不在app store内",
          boughtAt: "2018-02-04T16:00:00.000Z",
          link: "https://yeziapps.taobao.com",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/2/d9/a044b75b1ad150fbfbb3cc14c2ca5.png",
          remark: "",
          price: 688,
          type: "macOS"
        },
        {
          _id: "5a787e85e4290a7ea5910497",
          category: "图形与设计",
          name: "图片浏览器",
          description: "小巧的图片浏览器",
          boughtAt: "2015-10-12T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/%E5%9B%BE%E7%89%87%E6%B5%8F%E8%A7%88%E5%99%A8/id665540219?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/c/d5/8e4caefeb23ce58e402b51ce0d510.png",
          remark: "",
          price: 12,
          type: "macOS"
        },
        {
          _id: "5a787ed6e4290a7ea5910498",
          category: "摄影",
          name: "Diptic",
          description: "拼接照片用的，可以试试",
          boughtAt: "2015-10-12T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/diptic/id526546615?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/c/2d/7cd5560d2780f625bd831e21eb065.png",
          remark: "",
          price: 6,
          type: "macOS"
        },
        {
          _id: "5a787f20e4290a7ea5910499",
          category: "图形与设计",
          name: "iPaint",
          description: "Mac上优秀的画图工具",
          boughtAt: "2015-10-14T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/ipaint/id409676925?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/9/14/c90d08effbe04609135f50f025747.png",
          remark: "",
          price: 12,
          type: "macOS"
        },
        {
          _id: "5a787faae4290a7ea591049a",
          category: "图形与设计",
          name: "Hype 3",
          description: "需要内购，联系客服发送高级版本",
          boughtAt: "2018-02-05T15:59:56.820Z",
          link: "http://buy.yeziapp.com",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/26/5193be7bd4a1a1e377def73c2b0a3.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a78801b88ed3c35d757875b",
          category: "图形与设计",
          name: "Ember",
          description: "设计素材收集工具，很强大，老版本",
          boughtAt: "2015-10-14T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/8/23/d75f9bd331e0fcae479d314aa5d15.png",
          remark: "",
          price: 223,
          type: "macOS"
        },
        {
          _id: "5a78806d88ed3c35d757875d",
          category: "图形与设计",
          name: "Inboard",
          description: "设计素材收集工具",
          boughtAt: "2015-05-13T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/inboard-%E6%94%B6%E9%9B%86%E4%BD%A0%E7%9A%84%E7%81%B5%E6%84%9F/id944109819?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/b/fa/4752087e349e13029a55735a6d9c5.png",
          remark: "",
          price: 128,
          type: "macOS"
        },
        {
          _id: "5a8fa2806b4ecc5d7b4e980b",
          category: "效率",
          name: "OmniFocus 2",
          description: "联系客服提供激活码",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/5/e4/88c7002a5ea7305fa1dc47eecb71e.png",
          remark: "",
          price: 258,
          type: "macOS"
        },
        {
          _id: "5a8fa2c66b4ecc5d7b4e980c",
          category: "图形与设计",
          name: "OmniGraffle 7",
          description: "联系客服提供单独激活码",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/e/88/ec149b35092ae7c6af3b8be8e419a.png",
          remark: "",
          price: 1298,
          type: "macOS"
        },
        {
          _id: "5a8fa3026b4ecc5d7b4e980d",
          category: "效率",
          name: "OmniOutliner 5",
          description: "联系客服提供单独激活码",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/d/8d/281b2970d5a74f17c39278e9d2899.png",
          remark: "",
          price: 328,
          type: "macOS"
        },
        {
          _id: "5a8fa3236b4ecc5d7b4e980e",
          category: "商务",
          name: "OmniPlan 3",
          description: "联系客服提供激活码",
          boughtAt: "1999-12-31T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/5/df/5a047398095900196347741533f5b.png",
          remark: "",
          price: 1998,
          type: "macOS"
        },
        {
          _id: "5a8fa4066b4ecc5d7b4e980f",
          category: "图形与设计",
          name: "Affinity Designer",
          description: "专业的Mac图形设计工具",
          boughtAt: "2015-10-08T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/affinity-designer/id824171161?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/0/73/c51ecb39ccc8a21efebf7afd4f97a.png",
          remark: "",
          price: 256,
          type: "macOS"
        },
        {
          _id: "5a8fa4806b4ecc5d7b4e9810",
          category: "图形与设计",
          name: "Logoist",
          description: "Logo设计工具",
          boughtAt: "2017-11-09T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/logoist-3/id1247301872?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/e/b5/07d21205971b3a5b554f0df40ce35.png",
          remark: "",
          price: 0.01,
          type: "macOS"
        },
        {
          _id: "5a8fa5116b4ecc5d7b4e9811",
          category: "图形与设计",
          name: "Autodesk Graphic",
          description: "轻量级矢量绘图工具",
          boughtAt: "2015-10-20T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/autodesk-graphic/id404705039?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/1/5e/86fa07289b6b33b4661586cc4f34d.png",
          remark: "",
          price: 198,
          type: "macOS"
        },
        {
          _id: "5a8fa5546b4ecc5d7b4e9812",
          category: "图形与设计",
          name: "Pixave",
          description: "图片管理工具",
          boughtAt: "2015-11-24T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/pixave/id924891282?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/4/b1/c18b0a2b3eb8d43b6bcf286e8956c.png",
          remark: "",
          price: 98,
          type: "macOS"
        },
        {
          _id: "5a8fa5d06b4ecc5d7b4e9813",
          category: "摄影",
          name: "GifMaker",
          description: "从视频或图片中制作Gif的软件",
          boughtAt: "2015-09-27T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/gifmaker-create-a-gif-from-a-video-or-images/id1015930892?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/0/cd/defd2b910ac5b0851ba3e05caf793.png",
          remark: "",
          price: 12,
          type: "macOS"
        },
        {
          _id: "5a8fa6716b4ecc5d7b4e9814",
          category: "图形与设计",
          name: "SwordSoft Layout",
          description: "Mac平台的界面原型设计工具",
          boughtAt: "2016-01-20T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/swordsoft-layout/id438034858?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/1/e9/3f452f8536ead340131d75a20818b.png",
          remark: "",
          price: 45,
          type: "macOS"
        },
        {
          _id: "5a8fa7276b4ecc5d7b4e9816",
          category: "图形与设计",
          name: "Hexels 3",
          description: "六边形绘图设计工具，第三版本",
          boughtAt: "2016-05-02T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/hexels-3/id1087023846?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/2/bf/97773d2ee579af23262dd8bdc9007.png",
          remark: "",
          price: 318,
          type: "macOS"
        },
        {
          _id: "5a8fa7ee6b4ecc5d7b4e9819",
          category: "商务",
          name: "Fuel -Templates MS Office",
          description: "office模板软件",
          boughtAt: "2016-05-02T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/fuel-templates-for-ms-office/id897836426?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/c/6c/f99caf467d14821cb802dfebfdd1f.png",
          remark: "",
          price: 258,
          type: "macOS"
        },
        {
          _id: "5a8fa8976b4ecc5d7b4e981a",
          category: "图形与设计",
          name: "Fuel for iWork",
          description: "iWork模板",
          boughtAt: "2016-05-02T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/ef/0128e22238aacf101a22945bc1c6a.png",
          remark: "",
          price: 258,
          type: "macOS"
        },
        {
          _id: "5a8fa9466b4ecc5d7b4e981c",
          category: "图形与设计",
          name: "Fuel Templates for EverWeb",
          description: "网站设计模板",
          boughtAt: "2016-05-02T16:00:00.000Z",
          link: "",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/d/be/c59c1f297814fb768b8a1c0509923.png",
          remark: "",
          price: 128,
          type: "macOS"
        },
        {
          _id: "5a8fa99f6b4ecc5d7b4e981d",
          category: "图形与设计",
          name: "Pixa",
          description: "Mac上最好的图片管理工具",
          boughtAt: "2016-09-19T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/pixa/id527618971?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/2/5f/ebadbb187586ec4b713ea18c0d251.png",
          remark: "",
          price: 163,
          type: "macOS"
        },
        {
          _id: "5a8faa0c6b4ecc5d7b4e981e",
          category: "图形与设计",
          name: "Sketches Pro",
          description: "精美的画图工具",
          boughtAt: "2016-06-09T16:00:00.000Z",
          link:
            "https://itunes.apple.com/cn/app/sketches-pro/id1031566200?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/4/3a/529fe2b8dd5e718e0ce4a353de8a1.png",
          remark: "",
          price: 128,
          type: "macOS"
        },
        {
          _id: "5a8faa636b4ecc5d7b4e981f",
          category: "图形与设计",
          name: "Spectrum",
          description: "配色软件，操作简单，功能强大",
          boughtAt: "2016-12-12T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/spectrum/id518156125?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/a/02/836090e60faf773e47ad92b625aa4.png",
          remark: "",
          price: 128,
          type: "macOS"
        },
        {
          _id: "5a8faa9c6b4ecc5d7b4e9820",
          category: "摄影",
          name: "RAW Power",
          description: "处理RAW图片软件",
          boughtAt: "2017-02-18T16:00:00.000Z",
          link: "https://itunes.apple.com/cn/app/raw-power/id1157116444?mt=12",
          logo:
            "https://oss-cdn.yeziapp.com/projects/clover-server/md5/yezi/e/03/666626c1510bde599aee7242d304b.png",
          remark: "",
          price: 93,
          type: "macOS"
        }
      ]
    },
    computed: {
      computedList: function() {
        let data = {};
        this.list.forEach(item => {
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
</script>

{% endraw %}
