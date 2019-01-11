<body>
  <div id="app">加载中 ...</div>
  <script>
    window.$docsify = {
	 
      //切换页面后是否自动跳转到页面顶部
      auto2top: true,
      //是否启用封面
      coverpage: true,
      //是否允许执行文档里的 script 标签里的脚本 只执行第一个 script 如果 Vue 存在 则自动开启。
      executeScript: true,
      //是否启用左侧边栏
      loadSidebar: true,
      //是否启用自定义导航
      loadNavbar: true,
      //是否禁用 emoji 解析
      noEmoji: true,
      //小屏设备下合并导航栏到侧边栏
      mergeNavbar: true,
      //主题颜色设置
      //themeColor: '#3F51B5',
      //notFoundPage 未找到页面显示_404.md页面
      notFoundPage: false,
      //右上角github图标组件
      repo: 'https://github.com/time-fairy/',
      //最大支持渲染的标题层级为4
      maxLevel: 4,
      //设置生成目录的最大层级为2
      subMaxLevel: 2,
      //左侧边栏名称
      name: '时光精灵文档',
      //搜索模块开始
      search: {
        noData: {
          '/de-de/': 'Keine Ergebnisse!',
          '/zh-cn/': '没有结果!',
          '/': '没有结果!'
        },
        paths: 'auto',
        placeholder: {
          '/de-de/': 'Suche',
          '/zh-cn/': '搜索',
          '/': '请输入关键字开始搜索'
        }
      },
      //搜索模块结束
      //显示文档更新日期通过 {docsify-updated} 变量 并且格式化日期通过 formatUpdated
      formatUpdated: '{MM}/{DD} {HH}:{mm}',
      
    }
  </script>
  <script src="//unpkg.com/docsify/lib/docsify.min.js"></script>
  <script src="//unpkg.com/docsify/lib/plugins/search.min.js"></script>
  <script src="//unpkg.com/docsify/lib/plugins/emoji.min.js"></script>
  <script src="//unpkg.com/prismjs/components/prism-php.js"></script>
  <script src="//unpkg.com/prismjs/components/prism-bash.min.js"></script>
  <script src="//unpkg.com/prismjs/components/prism-markdown.min.js"></script>
  <script src="//unpkg.com/prismjs/components/prism-nginx.min.js"></script>
  
</body>