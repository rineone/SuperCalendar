# SuperCalendar
## 一个自定义日期。
* 因为导入原作者的库出现点问题，所以自己生成。
* 原作者Git链接：https://github.com/MagicMashRoom/SuperCalendar

导入方式：
   api 'com.github.rineone:SuperCalendar:1.1.0'
## 1.1修改

* 在原基础上加入，返回今日点的时候，返回点的位置
* 调用方式为：
* 1.刷新时，todayClick为布尔值，为是否点击今日按钮 calendarAdapter.notifyDataChanged(today,todayClick);
* 2.calendarAdapter.setOnCalendarTypeChangedListener加入一个内部接口：onCalendarToday(float x,float y)。此为接收今日点的位置