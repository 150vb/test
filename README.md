# mapxus-map-sample-ios

The sample for MapxusMapSDK.

* 创建地图

  1. 创建地图（代码）

     文件名：MXMCodingToShowMapViewController

     简介：通过代码创建地图

     详述：

     * 使用代码创建地图，并设置地图中心经纬度及缩放等级

  2. 创建地图（xib）

     文件名：MXMXibShowMapViewController

     简介：通过xib文件创建地图

     详述：

     * 使用xib拖拽控件创建地图，并设置地图中心经纬度及缩放等级

  3. 创建地图（指定初始建筑，楼层及建筑自适应边距）

     文件名：MXMBuildingInitializeViewController

     简介：创建地图时在设置的边距范围内最大化显示指定的建筑并切换到设置楼层

     详述：

     * 使用指定的建筑ID、楼层及建筑自适应边距创建参数类MXMConfiguration实例
     * 通过生成的MXMConfiguration实例初始化地图

  4. 创建地图（指定初始POI及地图缩放等级）

     文件名：MXMPOIInitializeViewController

     简介：创建地图时在地图中心显示指定的POI，并设置地图缩放等级

     详述：

     * 使用指定的POI、地图缩放等级创建参数类MXMConfiguration实例
     * 通过生成的MXMConfiguration实例初始化地图

* 地图交互

  1. 室内地图控件交互

     文件名：MXMIndoorControlViewController

     简介：室内地图控件的位置

     详述：

     * 是否一直隐藏室内地图控件
     * 设置室内地图控件位置：左边，右边，左上角，右上角，左下角，右下角

  2. 修改地图外观

     文件名：MXMMapAppearanceViewController

     简介：修改地图配色，标注语言及控制室外地图隐藏

     详述：

     * 是否隐藏室外地图
     * 更换地图样式
     * 更换地图标注语言

  3. 切换建筑的手势交互

     文件名：MXMSwitchingBuildingGesturesViewController

     简介：设置切换建筑手势

     详述：

     * 是否支持点击切换建筑
     * 是否支持移动到中心区域自动切换建筑

  4. 方法交互（切换室内场景）

     文件名：MXMFocusOnIndoorScenesViewController

     简介：代码设置聚焦的室内场景

     详述：

     * 设置地图聚焦的建筑与楼层
     * 设置聚焦效果：不缩放、通过动画缩放、无动画缩放
     * 设置建筑自适应边距

  5. 事件交互（点击）

     文件名：MXMClickEventListeningViewController

     简介：监听单击、长按地图事件，单击POI事件

     详述：

     * 单击地图，触发`- mapView:didSingleTappedAtCoordinate:`或`- mapView:didSingleTappedAtCoordinate:onFloor:inBuilding:`回调方法
     * 单击地图，触发`- mapView:didLongPressedAtCoordinate:`或`- mapView:didLongPressedAtCoordinate:onFloor:inBuilding:`回调方法
     * 长按地图回调
     * 长按地图回调
     * 点击地图空白处回调
     * 点击地图POI回调

  6. 事件交互（建筑或楼层切换）

     文件名：

     简介：

     详述：

     * 在切换建筑或楼层时，触发`- (**void**)mapView: didChangeFloor: atBuilding:`方法

  7. 事件交互（进出室内场景）

     文件名：

     简介：

     详述：

     * 在进出室内场景时，触发`- mapView: indoorMapWithIn: building: floor:`方法

* 在地图上绘制

  1. 按楼层显示的标注绘制

     文件名：

     简介：

     详述：

     * 切换建筑与楼层
     * 设置缩放方式
     * 设置缩放边距

* 室内定位效果展示

  1. 室内定位效果展示

     文件名：

     简介：

     详述：

     * 实时显示当前定位经纬度，楼层与水平精度
     * 切换不同的定位跟踪模式

* 地图数据检索

  1. 全球范围内建筑搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onBuildingSearchDone:response:`回调方法获取检索结果

  2. 指定区域内建筑搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例

     * 创建检索类的实例

     * 通过`- onBuildingSearchDone:response:`回调方法获取检索结果

  3. 周边建筑搜索

     文件名：

     简介：

     详述：

       * 创建检索参数类的实例
       * 创建检索类的实例
       * 通过`- onBuildingSearchDone:response:`回调方法获取检索结果

  4. 指定建筑ID搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onBuildingSearchDone:response:`回调方法获取检索结果

  5. 建筑内包含POI分类搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onBuildingSearchDone:response:`回调方法获取检索结果

  6. 指定建筑与楼层内POI搜索

     文件件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onPOISearchDone:response:`回调方法获取检索结果

  7. 指定区域内POI搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onPOISearchDone:response:`回调方法获取检索结果

  8. 周边POI搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onPOISearchDone:response:`回调方法获取检索结果

  9. 指定POI ID搜索

     文件名：

     简介：

     详述：

     * 创建检索参数类的实例
     * 创建检索类的实例
     * 通过`- onPOISearchDone:response:`回调方法获取检索结果

  10. 周边POI所在方位搜索

      文件名：

      简介：

      详述：

      * 创建检索参数类的实例
      * 创建检索类的实例
      * 通过`- onOrientationPOISearchDone:response:`回调方法获取检索结果

  11. 反地理编码检索

      文件名：

      简介：

      详述：

      * 创建检索参数类的实例
      * 创建检索类的实例
      * 通过`\- onGetReverseGeoCode: result: error:`回调方法获取检索结果

* 集成案例

  1. 路线规划与导航

     文件名：

     简介：检索起始点间的路线并实现路网吸附、缩短功能

     详述：

     * 创建检索参数类的实例
     * 

  2. Visual map

     文件名：

     简介：

     详述：

     * 查询选中室内场景是否有Visual map数据
     * 

  3. Siri shortcuts集成

     文件名：

     简介：

     详述：

     * 
