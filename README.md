# android图片加载框架Glide
开源项目地址:[https://github.com/open-android/Glide](https://github.com/open-android/Glide)

# 运行效果

  ![](static/sample.png)

  * 更多干货请下载app
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

###在AndroidManifest.xml中配置网络权限

	<uses-permission android:name="android.permission.INTERNET" />

