# mobileImgUpload
最近做了一个图片上传的项目（移动端）。放大，缩小，移动，裁剪与压缩图片。各种坑，虽说14年就有接触和制作过上传图片的项目，也了解了很多。总结下遇到和了解的问题：
  1）最大的坑就是系统为了安全的考虑屏蔽了上传文件的功能<input type="file">。三星、华为等android里webview不支持input file。
     这.....
  2）ios拍照上传后在传回客户端，图片旋转了，旋转了... 可以使用exif.js可以把每个exif信息参数给对应列出来
  3）ios拍照的图片裁剪，得到的图片是空白的，没有内容。
  大概就这些吧
还好有大神的代码，要不，就废了。

js中用到了load-image.js，github上的地址https://github.com/blueimp/JavaScript-Load-Image
