# roteImages 
### （开始考虑setDate毫秒级操作卡顿问题，所以使用了wepy框架，不过在原生上试过也不卡顿）
（小程序）手指对图片的拖动缩放和旋转
- 最近有一个需求，需要在小程序中实现对图片的 拖动  缩放 和 旋转，翻阅小程序文档，发现有一个 `movable-view` 的组件，可以实现 拖动和缩放，所以用这个组件实现了一遍这个功能，但是在真机上发现缩放的时候会有明显的顿挫感， 所以，又完整的实现了一遍功能

- 实现这个功能不难，试过了很多种方案和计算方法，都能最终实现，难点是在安卓端的卡顿问题，特别是在千元安卓机上，那卡顿。。简直是。。。，，所以，尝试了各种方法，最终，用原生方法在安卓机上也能思思顺滑般的操作了，（ `src/pages/nativeRota`）, index是使用原生组件写的，未优化
