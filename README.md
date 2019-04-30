# github_blog_source
1、hexo new "三步完成Github搭建个人博客"
为了更好的标识文章和防止重复，文章对应的markdown文件的命名应该遵循：YYYY-MM-DD-title 格式。
例如，今天是2019年3月3日，文章内容是与ES6有关。那么，文件名是2019-03-03-es6.md。
2、创建分类页：hexo new page categories  
  配置分类页：修改分类页对应的md文件(your-blog/source/categories/index.md)的Front-matter，为其添加type属性  

创建标签页：hexo new page tags

配置标签页：修改标签页对应的md文件(your-blog/source/tags/index.md)的Front-matter，为其添加type属性


$ hexo g -d
$ hexo d -g