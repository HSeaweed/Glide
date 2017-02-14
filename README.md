# android图片加载框架Glide
开源项目地址:[https://github.com/open-android/Glide](https://github.com/open-android/Glide)

 PS：如果觉得文章太长，你也可观看该课程的[视频](https://www.boxuegu.com/web/html/video.html?courseId=172&sectionId=8a2c9bed5a3a4c7e015a3bbffc6107ed&chapterId=8a2c9bed5a3a4c7e015a3aff408e0467&vId=8a2c9bed5a3a4c7e015a3b03c546046b&videoId=068DCD08470172549C33DC5901307461)，亲，里面还有高清，无码的福利喔

# 运行效果

  ![](static/sample.png)

* 爱生活,爱学习,更爱做代码的搬运工,分类查找更方便请下载黑马助手app
​

​
![黑马助手.png](http://upload-images.jianshu.io/upload_images/4037105-f777f1214328dcc4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
​
## 使用步骤

### 1. 在project的build.gradle添加如下代码(如下图)

        allprojects {
            repositories {
                ...
                mavenCentral() 
            }
        }


### 2. 在Module的build.gradle添加依赖

	   compile 'com.github.bumptech.glide:glide:3.7.0'
	   compile 'com.android.support:support-v4:19.1.0'

### 3. Imageview加载图片
​

	           Glide.with(context) //设置context
	          .load(url) //图片url地址
		        .placeholder(R.drawable.placeholder) //加载时显示的图片
		        .error(R.drawable.error) //加载错误显示的图片
		        .into(view);//图片显示的imageview

### 在AndroidManifest.xml中配置网络权限

	<uses-permission android:name="android.permission.INTERNET" />
	
	
* 详细的使用方法在DEMO里面都演示啦,如果你觉得这个库还不错,请赏我一颗star吧~~~

* 欢迎关注微信公众号

![](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)	

