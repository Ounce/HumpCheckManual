# 简介

&emsp;&emsp;驼峰溜放速度检算是驼峰调速系统设计重要步骤，是检查调速系统是否合理的重要手段。我中心早在80年代就开始研究利用计算机进行检算。先后开发过3至4个不同版本。使用时间最长的是徐正利和王立宁共同编写的，先后在alpha和MV机上运行，在上世纪90年代移植到PC机上，一直使用到现在。由于受到当时技术条件所限，PC版中停车顶的验算图保存有问题，驼峰部分不能实现动画显示。

&emsp;&emsp;新版本使用C++ Builder编写，充分吸取各版本的经验与教训，同时采用了一些新的科研成果。这个版本能够实现从驼峰一直到尾部全部动画显示；可以将车组预先设置到任意位置上，同时还可以设置速度；可以处理连挂或不连挂问题；根据国内外不同情况可以选择不同的单位制（公制或英制）。可以说这个系统可以满足减速顶调速系统检算过程中的所需全部要求。

## 系统结构

&emsp;&emsp;本系统大致可分为三个部分：

- 原始数据的管理；
- 模拟检算的动态显示；
- 输出统计结果、验算图；

## 功能和限制

&emsp;&emsp;主要功能除了正常驼峰检算模拟和尾部停车顶检算模拟外，还可以检算模拟特殊工况。

**功能**

- 可以根据需要将不同车组设置在不同的初始位置并设置不同的初始速度；
- 根据需要设置是否处理模拟车辆碰撞，碰撞后是否连挂的工况；
- 可以选用不同的单位制（公制和英制，不能转换数值），方便数据输入， 可以根据不同用户选用不同的单位制，方便客户了解检算模拟结果。
- 可以在检算模拟过程中动态显示车辆的速度和时间曲线。
- 可以在检算模拟过程中比较形象地动态显示车辆的运动状况。可以设置显示范围。
- 在驼峰验算图中选择车组的前端板、中心和后端板的速度曲线。
- 使用旧阻力计算公式。
- 方便的加密措施，授权用户可以不添加设备即可使用。

**限制**

- 控制系统简单，还不能适应复杂条件下微机可控顶调速系统的模拟，与实际的控制系统还有差距；
- 还不能直接设置各车组的溜放阻力和车场阻力。
- 车组必须是同一车型，同一载重。不过这对验算没有太大影响。

## 运行环境
&emsp;&emsp;本系统在Windows XP编写并测试，2013年转到Win7下，所以在该条件下一般不会有问题。但是由于在检算模拟过程中使用了Windows图形系统，因而对内存和CPU要求较高。（具体情况未测试）。

# 目录

[目录](summary.md)


