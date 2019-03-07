# SuperCalendar
## 一个自定义日期。
* 因为导入原作者的库出现点问题，所以自己生成。
* 原作者Git链接：https://github.com/MagicMashRoom/SuperCalendar

导入方式：
   api 'com.github.rineone:SuperCalendar:1.2.0'
## 1.1修改

* 在原基础上加入，返回今日点的时候，返回点的位置
* 调用方式为：
* 1.刷新时，todayClick为布尔值，为是否点击今日按钮 calendarAdapter.notifyDataChanged(today,todayClick);
* 2.calendarAdapter.setOnCalendarTypeChangedListener加入一个内部接口：onCalendarToday(float x,float y)。此为接收今日点的位置

## 1.2修改
 * 将获取到今日点和显示今日点圈分离，如图：
<div style = "float:center">
    <img src="http://www.one-cloudy.com//bg/jie.png" width="240">
<div/>
 * 例如这样点从大蓝点到小蓝点的动画
 * 调用方式：
 * 在onCalendarToday 中调用 toChangeTodayUi。即可显示今日点。不然只会获取今日点的位置坐标。