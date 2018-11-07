# canvas_CenterOfScaling
利用2d上下文context的`drawImage`方法绘制图像, 配合input[type=range]滑动杆的交互事件做出 中心缩放图片的demo  

需要注意两点:  
1. 每次缩放的绘制之前要`clearRect`清除一次画布  
2. [type=range] 的事件可以选择`onchange`, 但是有不完美的地方, 即 拖动滑竿松开鼠标才会重新绘制图像,  
而`onmousemove`事件可以解决上述问题