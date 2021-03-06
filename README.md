#SectorProgressBar

Examples
-------

Here are some examples of how these progressbars could look like:

![example](http://e.hiphotos.baidu.com/image/pic/item/3b292df5e0fe9925f89a13b032a85edf8cb171bf.jpg)

#Usage

Gradle
-------

This library now works with gradle and is available on the central maven repository. Just add the following repository to your app build.gradle:

    dependencies {
        // other repos ...
        compile 'com.github.znacloud:sectorprogressbar:1.0.0'
    }

Code
-------

After adding the gradle depedency from above you can go to your xml layout and add the following code for a squareprogressbar:

```xml
<com.github.znacloud.SectorProgressBar xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/spb_progress"
    android:layout_width="48dp"
    android:layout_height="48dp"
    app:progress="0"
    app:borderWidth="2dp"
    app:borderColor="@color/colorPrimary"
    app:sectorBackgroundColor="@color/colorAccent"
    app:sectorColor="@color/colorPrimaryDark"
    app:showTextProgress="true"/>
```

To set some basic settings use the following java-code:

```java
mCirclePbr = (SectorProgressBar) findViewById(R.id.spb_progress);
//set custom attribute
mCirclePbr.setSectorBackgroundColor(Color.parseColor("#55000000"));
mCirclePbr.setBorderColor(Color.GRAY);
mCirclePbr.setBorderWidth(4);
mCirclePbr.setShowTextPercent(true);
mCirclePbr.setProgress(20);
```

License
-------

    Copyright 2015-2015 Stephan Zeng
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
    

    
    
