<template>
  <div class="container" id="posts">
    <div class="post-preview" v-for="post in posts" :key="post.id">
      <div 
        :style="{ backgroundImage: 'url(' + post.thumbnailUrl + ')' }"
        class="post-preview-thumbnail">
      </div>
      <div class="post-preview-content">
        <h1>{{ post.title }}</h1>
        <p>{{ post.previewText }}</p>
        <a :href="post.site" style="text-decoration: none; color: blue;">こちら</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {
          title: "sunnY Vue",
          previewText: "こちらの作品はweather_APIを活用したアプリです。Vue.jsの学習始めに制作したものです。vue-cli3とBootstrapを使ってます。2020年6月に制作。",
          thumbnailUrl:
            "/sunny-vue.jpg",
          site: "https://sunny-vue-hinoizu.netlify.app/"
        },
        {
          title: "conVer",
          previewText: "こちらはVue.jsとNode.jsを使って制作しました。デプロイの仕方や環境変数の利用やpeerJsを使ってビデオチャット機能も入れる際にたくさん苦労しましたので個人的には一番思い入れのある制作物です。",
          thumbnailUrl:
            "/conver.chat.ver2.png",
          site: "https://conver-chat-hinoizu.herokuapp.com/"
        },
        {
          title: "ポートフォリオサイト",
          previewText: "こちらのポートフォリオサイトはNuxt.jsを使って制作しました。こだわりとしては、シンプルかつ青と緑がメインのデザインです。",
          thumbnailUrl:
            "/mysite.jpg",
          site: "/"
        },
        // {
        //   title: "taYlor",
        //   previewText: "vue-cli3とRailsを使って制作しました。個人アプリは白メインのデザインが多いと思い、紫メインにしました。途中で熱が覚めてしまい、デプロイ未済のまま放置しています。作成中に「これ無理してRailsでやらんでいいんじゃね？NodeとFirebaseの方が楽じゃね？」と感じたのが原因です。リンクはGitHubのリンクです。",
        //   thumbnailUrl:
        //     "/test3.png",
        //     // "/mysite.jpg",
        //   site: "https://github.com/hideokawahara/taylor"
        // },
         {
          title: "taYlor",
          previewText: "vue-cli3とRailsを使って制作しました。個人アプリは白メインのデザインが多いと思い、紫メインにしました。途中で熱が覚めてしまい、デプロイ未済のまま放置しています。作成中に「これ無理してRailsでやらんでいいんじゃね？NodeとFirebaseの方が楽じゃね？」と感じたのが原因です。リンクはGitHubのリンクです。",
          thumbnailUrl:
            "/test.png",
          site: "https://github.com/hideokawahara/taylor"
        },
        {
          title: "techInfo",
          previewText: "主に使ったのは、RailsとBootstrapです。大阪のプログラミング初学者の情報共有サイトのつもりで制作しました。これもデプロイ未済のまま熱が覚めてやめました。リンクはGitHubのリンクです。",
          thumbnailUrl:
            "/techinfo.png",
          site: "https://github.com/hideokawahara/rails_app"
        }, 
        {
          title: "red",
          previewText: "React.jsとFirebaseをメインに作成しました。これを作成する前にVueばっかり触ってたのでReactのコードの書き方がオシャレやなーと思いました。また、Firebase便利で感動しました。",
          thumbnailUrl:
            "/red.png",
          site: "https://red-react.web.app/"
        }, 
        {
          title: "rebecca",
          previewText: "ReactNativeとFirebaseを使って初めてモバイル系のアプリに挑戦しました。スマホのシミュレーターを用いながらの開発は新鮮さと衝撃がありました。デプロイはまだ未済で若干放置中です。リンクはGitHubのリンクです。",
          thumbnailUrl:
            "/rebecca.png",
          site: "https://github.com/hideokawahara/rebecca"
        },
        {
          title: "Victoria",
          previewText: "Node.jsメインに作成。こちらはpeerjsの練習がてらに作成。こちらの技術をconVerへ移していきました。開発は途中段階の都合上、リンクはこちらのサイトのホーム画面に飛びます。",
          thumbnailUrl:
            "https://www.pakutaso.com/shared/img/thumb/smokeIMGL8981_TP_V.jpg",
          site: "/"
        },
        {
          title: "Centaur",
          previewText: "こちらは今後作っていきたいと考えているものです。プログラミング学習コンテンツであり、現段階はただ構想を練っている段階でまだ具体的には作成していないですが、Webデベロッパーとしてのキャリアを歩みながら作成していきます。",
          thumbnailUrl:
            "/centaur.png",
          site: "/"
        }
      ]
    }
  }
}
</script>

<style scoped>
.post-preview {
  border-radius: 3px;
  box-shadow: 1px 1px 5px 1px rgba(0, 0, 0, 0.5);
  width: 90%;
  height: auto;
  margin: 1rem;
}
.post-preview-thumbnail {
  background-position: center;
  /* background-position:center bottom;  */
  background-size: contain;
  background-repeat:  no-repeat; 
  width: 100%;
  height: 10rem;
  margin-top: 1rem;
}
.post-preview-content {
  text-align: center;
  padding: 1rem;
  
}
@media (min-width: 35rem) {
  .post-preview {
    width: 25rem;
    /* word-break: break-all; */
  }
}
#posts {
  padding-top: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  /* word-break: break-all; */
  word-break: break-word;
}
@media (min-width: 35rem) {
  #posts {
    flex-direction: row;
    flex-wrap: wrap;
  }
}
</style>
